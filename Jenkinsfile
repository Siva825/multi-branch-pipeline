 pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo "build success"
            }
        }
         
            parallel{
                stage('test'){
                    steps{
                        echo "test success"
                    }
                }
                stage('deploy'){
                    steps{
                        echo "deploy success"
                    }
                }
            }
        
         
    }
}
