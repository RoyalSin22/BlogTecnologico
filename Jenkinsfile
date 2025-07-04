pipeline {
    agent any

    stages {
        stage('Clonar') {
            steps {
                git branch: 'develop', url: 'https://github.com/RoyalSin22/BlogTecnologico.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Ejecutando build...'
            }
        }
    }
}
