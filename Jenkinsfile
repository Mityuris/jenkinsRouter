pipeline {
    agent any
    tools {
        nodejs "NodeJS 20"
    }
    stages {
        stage ('build') {
            steps {
                npm install
            }
            steps {
            	npm run build
            }
        }
    }
    post {
    	always {
			npm test	
    	}
    }
}
