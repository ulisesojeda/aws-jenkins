pipeline {
	agent any
	stages {
		stage('Upload to AWS') {
				withAWS(credentials:'AKIATNP4XPJSEJRL55NJ (Static HTML publisher in AWS)') {
					s3Upload(file:'index.html', bucket:'aws-jenkins-2216', path:'/index.html')
				}
			}
		}
	}

