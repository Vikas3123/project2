pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "This is Build job"
            }
        }
        stage('Git') { 
            steps {
                git credentialsId: 'vikas', url: 'https://github.com/Vikas3123/project2.git'
            }    
        }
        stage('Maven') { 
            steps {
                sh label: '', script: 'mvn clean package'
            }
        }    
        stage('Test') { 
            steps {
                echo "This is Test job"
            }
        }
        stage('Deploy') { 
            steps {
                echo "This is Deploy job"
 
            }
        }
    }
}
