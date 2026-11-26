pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/AbhayVarshney19/Student-Registration.git'
            }
        }

        stage('Maven Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Success') {
            steps {
                echo 'Student Registration Build Successful!'
            }
        }
    }
}