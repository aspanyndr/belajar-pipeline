pipeline {
	agent any 
	stages{
		stage('build'){
			steps{
				sh 'docker build -t belajar-pipeline-2 .'
			}
		}
		stage('run'){
			steps {
				sh 'docker run --name belajar-pipeline-2 -d -p 5022:80 belajar-pipeline-2'
			}
		}
	}
}