pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'Maven-3.5.4') {
                    bat 'mvn clean compiles'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'Maven-3.5.4') {
                    bat 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven : 'Maven-3.5.4') {
                    bat 'mvn test'
                }
            }
        }
    }
}
