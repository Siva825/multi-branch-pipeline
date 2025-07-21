 pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo "build success"
            }
        }
        stage('scans'){
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
}
