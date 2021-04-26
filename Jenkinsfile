pipeline {
    agent any
    environment {
       NEW_VERSION = '1.1.0'
       SERVER_CRED = credentials('yantaq')
    }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                echo "building version ${NEW_VERSION}"
                echo "server cred ${SERVER_CRED}"
                sh '''
                   echo "Multiple shell steps works too"
                '''
            }
        }
    }
}
