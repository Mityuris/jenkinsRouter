pipeline {
    agent any
    tools {
        nodejs "NodeJS 20"
    }
    stages {
        stage('build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
    post {
    	always {
			sh 'npm test'	
    	}
    }
}
