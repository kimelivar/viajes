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
                sh './mvnw clean package'  // Para un proyecto Maven
            }
        }
        stage('Ejecutar Aplicación') {
            steps {
                sh 'java -jar target/viajes-0.0.1-SNAPSHOT.jar'  // Ajusta el nombre del JAR
            }
        }
    }
}
