pipeline {
    agent any

    stages {
        stage("build") {

            steps {
                echo 'Building app...'
                apt
            }
        }

        stage("test") {

            steps {
                echo 'Testing app...'
            }
        }
    }
}