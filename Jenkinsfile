 pipeline{
    agent any
    environment{
        name = 'siva'
    }
    stages{
        stage('build'){
            steps{
                echo "build success"
            }
        }
        stage('test'){
            when {
                allOf{
                    branch 'main'
                    environment name:'name',value:'siva'
                }
            }
            steps{
                echo "test success"
            }
        }
    }
}
