pipeline{
    agent any
    tools {nodejs "NodexJS"}
    stages{
        stage("Build"){
            steps{
                nodejs("NodexJS") {
                    sh 'npm install'
                    sh 'npm run build'
                }
            }
        }
        stage("Start"){
            steps{
                nodejs("NodexJS") {
                    sh 'npm run start'
                }
                echo "App started successfully"
            }
        }
    }
}
