pipeline {
    agent any

    stages {

        stage("install") {
            steps {
                echo 'Installing...'
                curl -sL https://rpm.nodesource.com/setup_14.x | sudo bash -
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