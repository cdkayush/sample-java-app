pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
	    	sh 'sudo chmod +777 ./mvnw'
	    	sh './mvnw install'
		sh './mvnw -Pprod clean verify'
            }
        }
        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }
    }
}

