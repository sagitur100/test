pipeline {
    agent {
      docker { 
	image 'python:3-slim' 
      } 
    }
    stages {
        stage('Build') {
            steps {
		pip install pytest
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
