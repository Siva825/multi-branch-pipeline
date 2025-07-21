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
                    environment name:'name', value:'siva'
                }
            }
            steps{
                echo "build success"
            }
        }
    }
}

