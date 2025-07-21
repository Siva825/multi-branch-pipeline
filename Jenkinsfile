 pipeline{
    agent any
    environment{
        name = 'siva'
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

