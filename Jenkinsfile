pipeline{
    agent any
    tools {nodejs "NodexJS"}
    stages{
        stage("Build"){
            steps{
                nodejs("NodexJS") {
                    sh 'npm install'
                    sh 'npm build'
                }
            }
        }
        stage("Start"){
            steps{
                nodejs("NodexJS") {
                    sh 'npm start'
                }
                echo "App started successfully"
            }
        }
    }
}
