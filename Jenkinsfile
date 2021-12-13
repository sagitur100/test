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
               sh 'python -m venv env; source ./env/bin/activate; python -m pip install pytest; python -m pytest'
	    }
        }
	stage('Deploy') {
	    steps {
		echo 'Deploying'
	    }
	}
    }
}
