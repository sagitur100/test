pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
		echo 'Building'
            }
        }
	stage('Test') {
	    steps {
		sh 'pytest'
	    }
        }
	stage('Deploy') {
	    steps {
		echo 'Deploying'
	    }
	}
    }
}
