 pipeline{
    agent {
        label 'java-slave'
    }
    environment{
        name = 'siva'
        course = "Devops"
    }
    triggers{
        cron('* * * * *')
    }
    stages{
        stage('build'){
            steps{
                echo "my name is ${name}"
                echo "course name is ${course}"
            }
        }
    }
}
