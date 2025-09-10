pipeline {
    agent any

    stages {
        stage('Clonar projeto') {
            steps {
                git branch: 'main', url: 'hhttps://github.com/mrscharlotte/jenkins.git'
            }
        }

        stage('Instalar dependências') {
            steps {
                sh 'npm install'
            }
        }

        stage('Rodar testes Cypress') {
            steps {
                sh 'npx cypress run'
            }
        }
    }
}
