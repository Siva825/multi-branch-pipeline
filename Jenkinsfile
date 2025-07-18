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
                branch 'feature'
                environment name: 'name', value:'siva'
            }
            steps{
                echo "build sucess"
            }
        }
    }
}
