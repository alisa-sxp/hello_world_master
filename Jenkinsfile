pipeline{
    agent any
    stages {
        stage('Build') {
            steps{
                echo 'This is a build step' 
            }
        }
        stage('Test') {
            steps{
                echo 'This is a test step master 11111'
                sleep(3000)
                /*master的改动*/
            }
        }
        stage('Deploy') {
            steps{
                echo 'This is a deploy stepmaster1111111111'
            }
        }
    }
    post {
        success {
            echo 'Here we kickoff run job testmaster2222222'
            build job: 'test'                                                                
               
            }
    }
}
