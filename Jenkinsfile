pipeline {
    agent any

    tools {
        maven "Maven"
    }
        stages {
             stage ('Testing Stage') {

            steps {
                    sh 'mvn test'
                }
            }
        


        stage('Build') {
            steps {
                dir('/var/lib/jenkins/workspace/multibranch-sample-app_master') {
                    sh 'mvn clean install'
                }
            }
        }
        }

    }
}
