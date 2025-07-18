 pipeline{
    agent {
        label 'java-slave'
    }
    environment{
        name = 'siva'
    }
    triggers{
        pollSCM('* * * * *')
    }
    stages{
        stage('build'){
            environment{
                course= 'Devops'
            }
            steps{
                echo "my name is ${name}"
                echo "course name : ${course}"
                echo "completed"
            }
        }
    }
}
