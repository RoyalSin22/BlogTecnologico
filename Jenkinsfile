pipeline {
    agent any

    stages {
        stage('Clonar') {
            steps {
                git branch: 'develop', url: 'https://github.com/RoyalSin22/BlogTecnologico.git'
            }
        }

        stage('Verificar estructura') {
            steps {
                echo '🔍 Verificando archivos HTML y CSS...'
                sh 'test -f html/index.html && echo "✅ index.html encontrado"'
                sh 'test -f styles/styles.css && echo "✅ CSS encontrado"'
                sh 'ls -R'  // Muestra toda la estructura de carpetas
            }
        }

        stage('Finalizado') {
            steps {
                echo '🎉 Validación de estructura completada con éxito.'
            }
        }
    }
}
