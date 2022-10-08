pipeline {
	agent any 
	stages{
		stage('build'){
			steps{
				sh 'docker build -t belajar-pipeline-1 .'
			}
		}
		stage('run'){
			steps {
				sh 'docker run --name belajar-pipeline-1 -d -p 5000:80 belajar-pipeline-1'
			}
		}
	}
}