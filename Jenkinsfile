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
                name: 'name', value:'siva'
            }
            steps{
                echo "build sucess"
            }
        }
    }
}
