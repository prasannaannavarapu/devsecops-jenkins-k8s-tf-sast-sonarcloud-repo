pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=reddybuggywebapp -Dsonar.organization=reddybuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5ab9cec94adb23137077f6121c5502710d39f06f'
			}
        } 
  }
}
