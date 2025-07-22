 pipeline{
    agent {
        label 'java-slave'
    }
    stages{
        stage('build'){
            steps{
                echo "build success"
            }
        }
        stage('Test'){
            steps{
                echo "Test success"
            }
        }
        stage('deploy'){
            steps{
                echo "deploy success"
            }
        }
    }
}

