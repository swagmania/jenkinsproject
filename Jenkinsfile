pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_8_4') {
                    sh 'mvn clean compile'
                }
            }
        }

        
        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'maven_3_8_4') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
