pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/Deep2553/lav_sms.git'
               
            }
        }
        stage('Test') {
            steps {
                sh './vendor/bin/phpunit'
               
            }
        }
    }
}
