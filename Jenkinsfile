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
                echo "my name is ${nam}" 
            }
        
        }
    }

    post{
        always{
            echo "result showing"
        }
        success{
            echo " build success"
        }
        failure{
            echo " build fail"
        }
}}
