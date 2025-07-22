 pipeline{
    agent{
        label'java-slave'
    }
    stages{
        stage('build'){
            steps{
                echo "build success"
            }
        }
        stage('test'){
            steps{
                echo "test success"
            }
        }
        stage('dockerbuild'){
            steps{
                echo "dockerbuild success"
            }
        }
        stage('devdeploy'){
            steps{
                echo "devdeploy success"
            }
        }
        stage('stagedeploy'){
            steps{
                echo "stagedeploy success"
            }
        }
        stage(' proddeploy'){
            /*options{
                timeout(time:300,unit:'SECONDS')
            }
            input{
                message"Doing prod deployments"
                ok'yes'
                submitter'siva'
            }*/
            steps{
                timeout(time:300,unit:'SECONDS'){
                    input message:"Doing prod deployments",ok:'yes',submitter:'siva'
                    echo "proddeploy success"
                }   
            }
        }
    }
}
