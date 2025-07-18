 pipeline{
    agent {
        label 'java-slave'
    }
    environment{
        name = 'siva'
    }
    stages{
        stage('build'){
            steps{
                echo "my name is ${name}"
            }
        }
    }
}
