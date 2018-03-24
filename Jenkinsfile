    pipeline {
        agent any
        stages {
            stage('Compile stage') {
                steps {
                    ('Maven_3.5.2'){
                        sh "mvn clean compile"
                }
            }
        }

             stage('testing stage') {
                 steps {
                    ('Maven_3.5.2'){
                        sh "mvn test"
                }
            }
        }

              stage('deployment stage') {
                  steps {
                    ('Maven_3.5.2'){
                        sh "mvn deploy"
                }
            }
        }

      }

    }
