pipeline {
    agent any  // Runs on any available agent

    tools {
        sonar-scanner 'sonar-scanner' // This refers to the configured tool in Jenkins, which is typically lowercase
    }

    environment {
        // Define environment variables if needed
        MY_VAR = 'Some value'
    }
    
    stages {
        stage('DIRECTORYbfgjknblkftklkfmklrmklr CONTENTS') {
            steps {
                // Runs a shell command and echoes a message
                sh 'ls -a'
                sh 'echo "THESE FILES CHANGCSFVEED"'
            }
        }
        stage('BUILDING') {
            steps {
                // Runs a shell command and echoes a message
                sh 'echo "HI BUILD PIPELINE"'
            }
        }
        stage('SONAR SCAN') {
            steps {
                // Run SonarQube Scanner to analyze the code

                sh '''
                    sonar-scanner \
                        -Dsonar.organization=developer-org-test \
                        -Dsonar.projectKey=developer-org-test_repo-1 \
                        -Dsonar.sources=. \
                        -Dsonar.host.url=https://sonarcloud.io
                '''
            }
        }
        stage('DEPLOYINg') {
            steps {
                // Example deploy step
                sh 'echo "HI DEPLOY PIPELINE"'
                // Add your deploy commands here (e.g., kubectl apply, aws deploy, etc.)
            }
        }
    }
}
