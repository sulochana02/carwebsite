pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/sulochana02/carwebsite.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Car Website'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
