pipeline {
	agent any
	stages {
		stage('Upload to AWS') {
				steps{
					withAWS(credentials:'df21a8f0-f14b-4cf6-a530-921c8cd7ccbf') {
						s3Upload(file:'index.html', bucket:'aws-jenkins-2216', path:'/static/index.html')
					}
				}
			}
		}
	}
	

