pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=skonph -Dsonar.organization=skonph -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=60bdbe808c5dea0d95c280629bbd7ffa7fc90d88'
			}
        } 
  }
}
