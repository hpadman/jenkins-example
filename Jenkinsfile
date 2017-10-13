pipeline {
    agent any

    tools {
        maven 'Maven 3.5.0'
        jdk 'jdk8'
    }

    stages {
        stage ('Compile Stage') {

            steps {
               'mvn clean compile'
            }
        }

        stage ('Testing Stage') {

            steps {
                mvn test
            }
        }


        stage ('Deployment Stage') {
            steps {
                'mvn deploy'
            }
        }
    }
}