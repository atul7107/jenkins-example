pipeline {
    agent any
    tools {
        maven 'TestMaven'
    }   
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(Maven : '3_5_0') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(Maven : '3_5_0') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(Maven : '3_5_0') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
