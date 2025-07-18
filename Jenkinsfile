 pipeline{
    agent {
        label 'java-slave'
    }
    environment{
        name = 'siva'
        course = "Devops"
    }
    triggers{
        buildPeriodically('* * * * *')
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
