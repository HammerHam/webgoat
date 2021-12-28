node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'Default Maven';
    withSonarQubeEnv(installationName: 'sq1') {
      sh "${mvn}/bin/mvn clean verify sonar:sonar -Dsonar.projectKey=WebGoat"
    }
  }
}
