pipeline {
    agent {
        dockerfile {
           filename 'dockerfile'
        }
    }
    stages {
        stage('Checkout') {
            steps{
                script{
                    git branch: 'main', url: 'https://github.com/dtkguiom/file_python.git'
                    sh "ls -lart ./*"
                }
            }
        }
        stage('exe') {
            steps{
                sh 'python devise.py'
            }
            
        }
    }
    
}
