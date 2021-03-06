pipeline {
    agent any
    tools {
            maven 'maven_3_6_3'
        }
    stages {
        stage ('Compile Stage') {

            steps {
                //tools(maven : 'maven_3_6_3') {
                    bat "mvn clean compile"
               // }
            }
        }

        stage ('Testing Stage') {

            steps {
                //tools(maven : 'maven_3_6_3') {
                    bat "mvn test"
               // }
            }
        }


        stage ('Deployment Stage') {
            steps {
                //tools(maven : 'maven_3_6_3') {
                    bat "mvn deploy"
                //}
            }
        }
    }
}