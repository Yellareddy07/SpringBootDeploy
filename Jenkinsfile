pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch:'main' 'https://github.com/Yellareddy07/SpringBootDeploy.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run Application') {
            steps {
                sh 'nohup java -jar target/demo-0.0.1-SNAPSHOT.jar &'
            }
        }
    }
}
