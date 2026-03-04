pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch:'main', url:'https://github.com/Yellareddy07/SpringBootDeploy.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        
        
    }
}
