pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
			steps {
                bat 'mvn test' 
            }
        }
    }
}