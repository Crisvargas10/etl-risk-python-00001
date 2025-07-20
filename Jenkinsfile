pipeline {
    agent any

    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'develop', url: 'https://github.com/Crisvargas10/etl-risk-python-00001.git'
            }
        }

        stage('Ejecutar ETL') {
            steps {
                sh 'python extract.py'
            }
        }
    }
}
