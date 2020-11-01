pipeline {
    agent any

    tools {nodejs "node"}

    stages {

        stage("install") {
            steps {
                sh 'npm install'
            }
        }

        stage("test") {

            steps {
                echo 'Testing app...'
                sh 'npm test'
            }
        }

        stage("build") {

            steps {
                echo 'Building app...'
                sh 'npm run build'
                sh 'aws s3 ls'
            }
        }


    }
}