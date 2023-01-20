pipeline {
  agent any
  tools { 
        maven 'Maven_3_6_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=damtotidevsecops -Dsonar.organization=damtotidevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e4de30c9a47e89b44600c62eb854706ae41dbeec'
			}
        } 
  }
}
