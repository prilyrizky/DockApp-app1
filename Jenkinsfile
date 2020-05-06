pipeline {
    agent none
    stages {
        stage('Build Image'){
            agent {dockerfile true}
            steps{
                sh "docker build -t tesNama -f Dockerfile ."
                sh "docker run -d -p 4000:80 tesNama"
            }
        }  
    }
}
