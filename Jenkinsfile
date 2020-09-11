pipeline {
    // agent any
    agent {label ' aws-ecs' }

    stages {
        // Build General Dependencies
        stage ( ' Dependencies ' ) {
            steps {
                sh " apt-get update -y "
                sh " apt-get install -y python3-pip "
                sh " pip3 --version "
                sh " pwd "
                sh " ls "
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
