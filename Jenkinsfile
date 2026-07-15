pipeline {
    agent none

    stages {

        stage('Build Java Application') {
            agent {
                label 'linux && java'
            }

            steps {
                echo 'Running on Java Agent'

                sh 'java -version'
                sh 'mvn -version'

                sh 'mvn clean package'
            }
        }

    }
}