pipeline {
    agent any
    tools{
        maven 'Maven3_9_8'
    }
    stages{
        stage('Checkout'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/vramprasad/tf-jenkins.git']]])
            }

        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
    } // End of stages 
} // End of pipeline