pipeline {
    agent any

    tools {nodejs "node"}

    stages {

        stage("install") {
            steps {
                sh 'npm config ls'
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