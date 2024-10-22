
//junit
pipeline{
    agent any
    stages{
        
        stage("clone repo")
        {
            steps{
                git branch:'main',url:'https://github.com/Shabila-khan/Jenkins.git'
            }
        }
        
        stage('Install dependencies'){
            steps{   
                sh 'npm install'
            }
        }
        
        stage('Start the  application'){
            input{
                message 'you really want to start'
                ok "Click on ok"
                submitter "Shabila"
            }
            steps{
                sh 'npm start'
            }
        }
    }
}