pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                tools(maven : 'maven_3_6_3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                tools(maven : 'maven_3_6_3') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                tools(maven : 'maven_3_6_3') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}