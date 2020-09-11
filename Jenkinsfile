pipeline {
    // agent any
    agent {label ' aws-ecs' }

    stages {
        // Build General Dependencies
        stage ( ' Dependencies ' ) {
            steps {
                sh " apt-get install -y "
                sh " apt install python3-pip "
                sh " pip3 --version "
                sh " pwd"
                sh "ls"
            }
        }

        // Deploy
        stage ( ' Deploy ' ) {
            steps {
                echo ' Fake Deploy '
            }
        }
    }

    post {
        always {
            // Clean Workspace
            cleanWs ()
        }
    }
}
