pipeline{
    agent {
        label 'java-slave'
    }
    stages{
        stage('build'){
            steps{
                echo "build success"
                sh 'hostname -i'
            }
            post{
                always{
                    echo "build is running" 
                }
                success{
                    echo "build successful"
                }
                failure{
                    echo "build failure"
                }
            }
        }
    }
}
