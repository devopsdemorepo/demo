pipeline {
    
    agent any
    
    tools {
        maven "maven"
        }
    stages {
		stage('prepare') {
            steps {
                sh "mvn package"
            }
		}
    }
}
