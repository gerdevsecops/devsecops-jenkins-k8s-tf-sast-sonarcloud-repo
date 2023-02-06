pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gerdevsecops_project -Dsonar.organization=gerdevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0a0f024f2b9cd138188c02a864bdf67effd7e265'
			}
        } 
  }
}
