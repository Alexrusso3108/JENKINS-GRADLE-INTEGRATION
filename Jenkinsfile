 
pipeline { 
    agent any 
    stages { 
        stage('Checkout') { 
            steps { 
                git 'https://github.com/JENKINS-GRADLE-INTEGRATION.git' 
            } 
        } 
        stage('Build') { 
            steps { 
                sh 'mvn clean install' 
            } 
        } 
        stage('Test') { 
            steps { 
                sh 'mvn test' 
            } 
        } 
        stage('Deploy') { 
            steps { 
                echo 'Deploying application...' 
            } 
        } 
    } 
} 
