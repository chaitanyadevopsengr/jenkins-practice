pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo "Current Branch: ${env.BRANCH_NAME}"
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo "Deploy only from main"
            }
        }

    }
}
