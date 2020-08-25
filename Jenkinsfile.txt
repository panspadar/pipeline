pipeline {
    agent any
    environment {
        PROJECT_NAME = "V ZHOPY RAZ ILI VILKOU V GLAZ"
        OWNER_NAME = "Pahom"
    }
    stages {
        stage('Hello1') {
            steps {
                echo 'Hello World PIYPIY'
            }
        }
        stage('Hello2') {
            steps {
                echo 'Hello World PAYPAY'
                sh ''' 
                echo "pervyu"
                echo "vtoroy"
                echo "tretuy"
                '''
            }
        }
        stage('Hello3') {
            steps {
                echo 'Hello NAXYU'
                echo "Hello ${OWNER_NAME}"
                echo "Vibirau ${PROJECT_NAME}"
            }
        }
    }
}
