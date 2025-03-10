pipeline {
    agent any
    tools {
        nodejs "NodeJS 20"
    }
    stages {
        stage ('build') {
            steps {
                npm install
                npm run build
            }
        }
    }
    post {
		npm test
    }
}
