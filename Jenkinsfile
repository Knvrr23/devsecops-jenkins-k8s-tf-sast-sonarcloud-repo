pipeline {
 agent any
 tools {
       maven 'Maven_3_8_4' 
   }
  stages{
   stage('CompileandRunSonarAnalysis') {
           steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9325586a8f1d1adf470b908a46156f5844'
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp123 -Dsonar.organization=buggywebapp123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fdcc533ace7a9b68714e0cf7ebdf438ac6d569bd'
			}
       }
 }

