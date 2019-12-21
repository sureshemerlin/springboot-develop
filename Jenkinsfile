pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat 'mvn spring-boot:run'
                echo "Application Started successfully...."
            }
        }
    }
}