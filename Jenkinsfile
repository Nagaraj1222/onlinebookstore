pipeline{
    agent any
    tools{
        maven:'maven'
    }
    Stages{
        stage('git checkout'){
            step{
                git branch: 'feature/2026.02.08', url: 'https://github.com/Nagaraj1222/onlinebookstore.git'
            }
        }
        stage('clean and install'){
            step{
                sh: 'mvn clean and install'
            }
        }
        stage('package'){
            step{
                sh: 'mvn package'
            }
        }
    }
}