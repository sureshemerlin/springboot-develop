pipeline {
    agent { label 'deve' }
    stages {
        stage('build') {
            steps {
                mvn clean compile
                echo "mvn spring-boot:run"
            }
        }
    }
}