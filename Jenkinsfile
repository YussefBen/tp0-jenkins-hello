pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/YussefBen/tp0-jenkins-hello.git'
            }
        }

        stage('Run app.py') {
            steps {
                echo "Exécution du script app.py"
                bat "python app.py"
            }
        }

        stage('Run calculatrice.py') {
            steps {
                echo "Exécution du script calculatrice.py"
                bat "python calculatrice.py"
            }
        }
    }
}
