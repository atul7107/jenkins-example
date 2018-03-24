    pipeline {
        agent any
        stages {
            stage('Compile stage') {
                steps {
                    maven('Maven_3.5.2'){
                        sh "mvn clean compile"
                }
            }
        }

             stage('testing stage') {
                 steps {
                    maven('Maven_3.5.2'){
                        sh "mvn test"
                }
            }
        }

              stage('deployment stage') {
                  steps {
                    maven('Maven_3.5.2'){
                        sh "mvn deploy"
                }
            }
        }

      }

    }
