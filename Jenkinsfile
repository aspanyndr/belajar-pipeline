pipeline {
	agent any 
	stages{
		stage('build'){
			steps{
				sh 'docker build -t belajar-pipeline-3 .'
			}
		}

		stage('clean up'){
			steps{
				sh 'docker stop belajar-pipeline-3 || true'
				sh 'docker rm belajar-pipeline-3 || true'
			}
		}
		stage('run'){
			steps {
				sh 'docker run --name belajar-pipeline-3 -d -p 5023:80 belajar-pipeline-3'
			}
		}
	}
}