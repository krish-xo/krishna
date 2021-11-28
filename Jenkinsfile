pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Git') {
            steps {
                git branch: 'main', credentialsId: '19060f75-61a0-4c2d-9afe-47e0a9e58159', url: 'https://github.com/krish-xo/project_code.git'
            } 
        }
        stage('Mail') {
            steps {
                mail bcc: '', body: 'Sending Email through scripting', cc: 'muralikrishnasarvepalli2@gmail.com', from: '', replyTo: '', subject: 'Jenkins', to: 'muralikrishnasarvepalli@gmail.com'
            }
        }
        stage('message') {
            steps {
                echo 'Succesfully completed'
            }
        }
    }
}
