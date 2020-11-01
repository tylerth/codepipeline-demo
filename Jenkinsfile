pipeline {
    agent any

    tools {nodesjs "node"}

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