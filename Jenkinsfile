pipeline {
    agent any
    environment {
       NEW_VERSION = '1.1.0'
    }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                echo "building version ${NEW_VERSION}"
                sh '''
                   echo "Multiple shell steps works too"
                '''
            }
        }
    }
}
