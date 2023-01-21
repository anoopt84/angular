pipeline {
    agent any
    stages {
        stage('Checkout Stage') {
            steps {
                git credentialsId: 'dba44211-5114-45c7-a8ae-9bb0b714c83c', url: 'https://github.com/anoopt84/angularlab.git', branch: 'master'
            }
        }
        stage('npm Install Stage') {
            steps {
                bat 'npm install'
            }
        }
		stage('Build Stage') {
            steps {
                bat 'npm run build'
            }
        }
    }
}