pipeline {
  agent any
  tools { 
        maven 'Maven_3'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mysonarcloud1 -Dsonar.organization=mysonarcloud1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=3d33337c3f31da9c636461c6770ff453dbc3e4f3'
			}
        } 
  }
}
