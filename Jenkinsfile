pipeline {
    agent any

    stages {

        stage("install") {
            steps {
                echo 'Installing...'
                sh 'curl -sL https://deb.nodesource.com/setup_12.x | bash -'
                sh 'apt install -y nodejs'
                sh 'curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -'
                sh 'echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list'
                sh 'apt install --no-install-recommends yarn'
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