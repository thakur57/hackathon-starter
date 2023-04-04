pipeline {
    agent any

    stages {
        stage('run docker file') {
            steps {
                  sh ("docker build -t thakur57/nodeapp:latest .")
            }
        }
    }
}
