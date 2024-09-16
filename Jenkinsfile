pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/Deep2553/lav_sms.git'
                sh 'composer install'
                sh '.env'
                sh 'php artisan key:generate'
            }
        }
        stage('Test') {
            steps {
                sh './vendor/bin/phpunit'
                sh 'composer install'
            }
        }
    }
}
