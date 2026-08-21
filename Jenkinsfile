pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code déjà récupéré par Jenkins via SCM checkout automatique'
            }
        }

        stage('Info') {
            steps {
                sh 'echo "Build number: ${BUILD_NUMBER}"'
                sh 'echo "Workspace: ${WORKSPACE}"'
                sh 'pwd && ls -la'
            }
        }

        stage('Test') {
            steps {
                echo 'Pipeline fonctionnel — prêt pour la suite du lab'
            }
        }
    }

    post {
        success {
            echo 'Build réussi !'
        }
        failure {
            echo 'Build en échec — vérifier les logs ci-dessus'
        }
    }
}// test webhook Fri Aug 21 19:31:00 +01 2026
