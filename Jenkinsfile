pipeline {
    agent any
    stages {
        stage('Clean Workspace') {
            steps {
                deleteDir()  // Clean up the workspace
            }
        }
        stage('Clone Repository') {
            steps {
                // Clone the repository from GitHub, explicitly using the 'main' branch
                git branch: 'main', url: 'https://github.com/ShahwaizAliKhan/Jenkins-CICD.git'
            }
        }
        stage('Build') {
            steps {
                echo 'No build steps required for static website.'
            }
        }
        stage('Test') {
            steps {
                echo 'No tests required for static website.'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying static website...'
                bat '''
                    echo Deploying static website...
                    REM Add your deployment steps here
                    '''


            }
        }
    }
}
