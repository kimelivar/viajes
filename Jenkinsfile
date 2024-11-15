pipeline {
    agent any
    stages {
        stage('Clonar Repositorio') {
            steps {
                git 'https://github.com/kimelivar/viajes.git'  // Reemplaza con tu URL de GitHub
            }
        }
        stage('Compilar y Construir') {
            steps {
                bat './mvnw clean package'  // Usar 'bat' en lugar de 'sh' en Windows
            }
        }
        stage('Ejecutar Aplicación') {
            steps {
                bat 'java -jar target/viajes-0.0.1-SNAPSHOT.jar'  // Usar 'bat' en lugar de 'sh' en Windows
            }
        }
    }
}
