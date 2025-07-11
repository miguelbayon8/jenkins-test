pipeline {
    agent any

    stages {
        stage('Preparar entorno') {
            steps {
                sh 'echo "Preparando entorno de trabajo..."'
                sh 'mkdir -p build'
            }
        }

        stage('Instalar dependencias') {
            steps {
                sh 'echo "Instalando dependencias (simulado)..."'
                sh 'sleep 2'  // Simula instalación
            }
        }

        stage('Compilar') {
            steps {
                sh 'echo "Compilando proyecto..."'
                sh 'touch build/app'
            }
        }

        stage('Pruebas') {
            steps {
                sh 'echo "Ejecutando pruebas..."'
                sh 'exit 0'  // Simula pruebas exitosas (cambia a 1 para forzar error)
            }
        }

        stage('Despliegue') {
            steps {
                sh 'echo "Desplegando aplicación..."'
                sh 'mv build/app /tmp/app-desplegado'
            }
        }
    }
}
