pipeline {
    agent any // This specifies the agent where the pipeline will execute, 'any' means it can run on any available agent

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from your Git repository
                git 'https://github.com/prasanna1devops/maven-project1'
            }
        }

        stage('Build') {
            steps {
                // Run Maven commands to build the project
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run Maven test commands
                sh 'mvn test'
            }
        }
    }
}

        
