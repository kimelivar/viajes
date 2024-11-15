pipeline {
    agent any
    stages {
        stage('Clonar Repositorio') {
            steps {
                git 'https://github.com/kimelivar/viajes.git'
            }
        }
        stage('Compilar y Construir') {
            steps {
                sh './mvnw clean package'
            }
        }
        stage('Ejecutar Aplicación') {
            steps {
                sh 'java -jar target/viajes-0.0.1-SNAPSHOT.jar
.jar'
            }
        }
    }
}
