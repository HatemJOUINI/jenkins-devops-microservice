// SCRIPTED

// DECLARATIVE
pipeline {
	//agent any
	agent { docker { image 'node:13.8'}}
	stages {
		stage('Build') {
			steps {
				    // sh 'mvn --version'
					sh 'node --version'
                    echo "Build"
			}
		}
		stage('Test') {
			steps {
		            echo "Test"
			}
		}
		stage('Test integraion') {
			steps {
		            echo "Test integraion"
			}
		}
	} 
	
	post {
		always {
			echo 'Im awesome i run always'
		}

		success {
			echo 'I run when u are successful'
		}
		
		failure {
			echo 'I run when u fail'
		}
	}
		
}

