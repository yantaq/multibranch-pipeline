pipeline {
    agent any
    parameters {
       string(name: 'VERSION', defaultValue: '', description: 'version to deploy on prod') 
       choice(name: 'VERSION', choices: ['1.1.0', '1.3.0'])
    }
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
