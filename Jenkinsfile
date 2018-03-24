pipeline {
    agent any
    tools {
        maven 'Maven_3.5.2'
    }   
    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5.2') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5.2') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'maven_3_5.2') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
