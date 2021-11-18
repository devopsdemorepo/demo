pipeline {
    
    agent any
    
    tools {
        maven "maven"
        }
    stages {
		stage('build') {
            steps {
                sh "mvn package"
            }
	}
    }

	
	
	post {
        always {          
            archiveArtifacts artifacts: "**/target/*.war", onlyIfSuccessful: true
            
  
        }
    }
}

