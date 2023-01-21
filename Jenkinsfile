pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapp191 -Dsonar.organization=buggywebapp191 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=68bbca8ecdff505686bc3e67db71d53dc0edb563'
			}
        } 
  }
}
