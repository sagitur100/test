pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                chmod +x ./add.py ./test_add.py 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
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
