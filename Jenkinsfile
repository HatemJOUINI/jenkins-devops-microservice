// SCRIPTED

// DECLARATIVE
pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
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
	} post {
		always {
			echo 'Im awesome i run always'
		}

		Success {
			echo 'I run when u are successful'
		}

		
		Failure {
			echo 'I run when u fail'
		}
	}
		
}

