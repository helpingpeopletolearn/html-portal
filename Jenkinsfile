pipeline {
	agent any

	stages {
		stage('Fecth code') {
			steps {
				git branch: 'main', url: 'https://github.com/helpingpeopletolearn/html-portal.git'
			}
		}
		stage('Install Websever') {
			steps {

				sh 'sudo apt install apache2 -y'
			}
		}
		stage('Deploy application') {
			steps {
				sh 'sudo cp -R * /var/www/html/'
			}
		}	

	}

}
