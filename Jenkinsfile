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
                bat 'mvnw.cmd clean package'  // Usar 'mvnw.cmd' en Windows
            }
        }
        stage('Ejecutar Aplicación') {
            steps {
                bat 'java -jar target/viajes-0.0.1-SNAPSHOT.jar'  // Usar 'bat' para ejecutar en Windows
            }
        }
    }
}

