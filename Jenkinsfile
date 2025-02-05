pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=akondareddyguru -Dsonar.organization=akondareddyguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f159f2605f57256011ae667ce9bb8a56cb21944b'
			}
        } 
  }
}
