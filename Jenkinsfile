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
                    environment name:'names', value:'siva'
                }
            }
            steps{
                echo "build success"
            }
        }
    }
}
