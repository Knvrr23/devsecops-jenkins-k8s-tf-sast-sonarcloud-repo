pipeline {
 agent any
 tools {
       maven 'Maven_3_8_4' 
   }
  stages{
   stage('CompileandRunSonarAnalysis') {
           steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp123 -Dsonar.organization=buggywebapp123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fdcc533ace7a9b68714e0cf7ebdf438ac6d569bd'
			}
       }
 }

