// SCRIPTED

// DECLARATIVE
pipeline {
	//agent { docker { image 'node:13.8'}}
	agent any
    environment { 
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	} 
	stages {
		stage('Build') {
			steps {
				    sh 'mvn --version'
					sh 'docker version'
                    echo "Build"
					echo "PATH - $PATH"
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

