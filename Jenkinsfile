pipeline {
    agent {
      docker { 
	  image 'python:3-slim' 
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
                python pip install pytest
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
