 pipeline {
    agent any
    environment{
        name = 'siva'
        roll no = '26'
    }
    stages{
        stage('build'){
            environment{
                course = 'mca'
            }
            steps{
                echo "my name is ${name}"
                echo "my roll no is ${roll no}"
                echo "class : ${course}"
            }
        }
    }
}
