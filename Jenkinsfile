pipeline {
    agent {
      docker { 
	  image 'python:3-alpine' 
      } 
    }
    stages {
        stage('Build') {
            steps {
		echo 'Building..'
            }
        }
	stage('Test') {
	    steps {
               sh 'python -m pytest'
	    }
        }
	stage('Deploy') {
	    steps {
		echo 'Deploying'
	    }
	}
    }
}
