pipeline {
    agent any
    tools {
        maven 'TestMaven'
    }   
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven) {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven) {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(mave) {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
