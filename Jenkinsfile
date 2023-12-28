pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp12282023 -Dsonar.organization=asgbuggywebapp12282023 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1052326de89cdca55d50e78bbdc13fc9c2128892'
			}
        } 
  }
}
