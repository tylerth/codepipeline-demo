pipeline {
    agent any

    stages {

        stage("install") {
            steps {
                echo 'Installing...'
                sh 'curl -sL https://rpm.nodesource.com/setup_14.x | bash -'
            }
        }

        stage("build") {

            steps {
                echo 'Building app...'
            }
        }

        stage("test") {

            steps {
                echo 'Testing app...'
            }
        }
    }
}