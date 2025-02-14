pipeline  {
    agent { label 'maven-agent' }
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/abdullasd14301/opsabdul.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
