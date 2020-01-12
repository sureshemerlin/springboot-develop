


String checkOutFrom(input) {
        print "Hello World  ${input}"
    }

String checkOutFrom(input) {
        print "Hello World  ${input}"
    }

pipeline {
    agent any

    stages {
        stage('build') {
            steps {
            def z = checkOutFrom("ddddddddddddddddddd")
                bat 'mvn spring-boot:run'
                echo "Application Started successfully...."
            }
        }
        stage('purge') {
            steps {
                def pipeline = checkOutFrom("uuuuuuuuuuuuuuu")
            }
        }
    }
      post {
            always {
                echo 'Pipeline executed..'
            }
            success {
                echo 'Deployment is successful'
            }
            failure {
                echo 'Deployment is failed'
            }
            unstable {
                echo 'This will run only if the run was marked as unstable'
            }
            changed {
                echo 'This will run only if the state of the Pipeline has changed'
                echo 'For example, if the Pipeline was previously failing but is now successful'
            }
        }
}