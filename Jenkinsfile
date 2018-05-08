pipeline {
    agent any
    tools {
            maven 'LOCALMAVEN'
            jdk 'jdk8'
    }

    stages {
        stage('Compile Stage') {
            steps
                 {
                    bat 'sh -c mvn validate'
                }

        }


        stage('Testing Stage') {
            steps {

                    bat 'sh -c mvn test'
                }

        }

        stage('Deployment Stage') {
            steps {
                    bat 'sh -c mvn deploy'
                }

        }
    }
}