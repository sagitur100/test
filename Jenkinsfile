pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
		echo 'Building'
		python pip install pytest
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
