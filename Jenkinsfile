pipeline {
  agent any
  tools { 
        maven 'maven3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=demotesttelus -Dsonar.organization=demotesttelus -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=cda6fa602ebb9db4a5bfbe701c214e343f8aa970'
			}
        } 
  }
}
