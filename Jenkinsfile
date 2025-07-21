// anyOf
pipeline{
    agent any
    environment{
        name = 'siva'
    }
    triggers{
        cron('* * * * *')
    }
    stages{
        stage('build'){
            when{
                anyOf {
                    branch 'mains'
                    environment name:'name', value:'siva'
                }
            }
            steps{
                echo "build success"
            }
        }
    }
}
