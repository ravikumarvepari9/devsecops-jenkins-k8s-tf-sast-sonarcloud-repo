pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ravibuggywebapp -Dsonar.organization=ravibuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8cce85e9f8aa6f310d476765858a77d46165fc47'
			}
        } 
  }
}
