 pipeline{
    agent{
        label 'java-slave'
    }
    environment{
        name ='siva'
    }
    triggers{
        githubPush()
    }
    stages{
        stage('build'){
            when{
                environment name: 'name', value:'siva'
            }
            steps{
                echo "build sucess"
            }
        }
    }
}
