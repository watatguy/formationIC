pipeline {
    agent any
    stages {
		stage('Code Quality') { 
            steps {
                bat 'mvn sonar:sonar' 
            }
        }
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
        }
		stage('Test') { 
            steps {
                bat 'mvn test' 
            }
        }
    }
}