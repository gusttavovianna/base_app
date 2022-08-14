node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool "sonarScanner';
    withSonarQubeEnv('SonarQube') {
        sh "${scannerHome}/sonar-scanner"
     }
   }
}