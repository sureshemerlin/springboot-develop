pipeline {
    agent { label 'deve' }
    stages {
        stage('build') {
            steps {
                //echo "Hello World!"
                'mvn spring-boot:run'
            }
        }
    }
}