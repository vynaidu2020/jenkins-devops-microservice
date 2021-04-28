//SCRIPTED

//DECLARATIVE
pipeline {
        agent any
       
        stages {
            stage('Build') {
                steps {
                        //sh 'mvn --version'
                        echo "Build"
						echo "$PATH"
						echo "BUILD_NUMBER - $env.BUILD.NUMBER"
						echo "BUILD_ID - $env.BUILD_ID"
						echo "JOB_NAME - $env.JOB_NAME"
						echo "BUILD_TAG - $env.BUILD_TAG"
						echo "BUILD_TAG - $env.BUILD_URL"
                }
            }
            stage('Test') {
                steps {
                        echo "Test"
                }
            }
            stage('Integration Test') {
                steps {
                        echo "Integration Test"
                }
            }
        }
        post {
            always {
                echo "I am awesome. I run always"
            }
            success {
                echo "I run when you are run successful"
            }
            failure {
                echo "I run when you fail"
            }
        }
}
