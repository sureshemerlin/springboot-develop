


String checkOutFrom(input) {
        print "Hello World  ${input}"
        return "ffffffff"
    }



pipeline {
    agent any

    stages {
     stage('Jacoco code coverage') {
                             steps {
                                checkOutFrom("Jacoco code coverage")
                                 bat 'mvn test'
                                 echo "Application Started successfully...."
                             }
                         }

        stage('sonarscan') {
                     steps {
                         checkOutFrom("sonarscan")
                         bat 'mvn test sonar:sonar'
                        echo "Application Started successfully...."
                                         }
                                     }
        stage('build') {
            steps {
               checkOutFrom("build")
                bat 'mvn spring-boot:run'
                echo "Application Started successfully...."
            }
        }
        stage('purge') {
            steps {
                  checkOutFrom("uuuuuuuuuuuuuuu")
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