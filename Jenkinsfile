pipeline {
	//agent any 
	agent { docker { image 'maven:3.6.3'} }
	stages {
			stage('Build') {
				steps {
					sh 'mvn --version'
					echo "Build"
				}		
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('intefration-Test') {
			steps {
				echo "integration Test"
			}
		} 
	}

	 post {
		always {
			echo 'i am awesome'
		}
		success {
			echo 'i run you are success'
		}
		failure {
			echo 'i run you are fail'
		}
	}
	
}
