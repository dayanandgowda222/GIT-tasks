pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'

            }
        }
    }
    post {
        success {
            mail bcc: '', body: 'hi i am jenkins', cc: '', from: '', replyTo: '', subject: 'build success', to: 'sharathyp25@gmail.com'
        }
        failure {
            mail bcc: '', body: 'hi i am jenkins', cc: '', from: '', replyTo: '', subject: 'build failed', to: 'sharathyp25@gmail.com'
        }
    }
}
