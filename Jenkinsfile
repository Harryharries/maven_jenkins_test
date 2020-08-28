pipeline{
agent any 
    tools {
    maven 'Maven'
    }
    stages {
        stage('clone repo') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"
            }
        }
        stage('---package---') { 
            steps {
                sh "mvn package" 
            }
        }
    }
}
