pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
	    	sh './mvnw install'
		sh './mvnw -Pprod clean verify'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "This stage will run tests."'
            }
        }
    }
}

