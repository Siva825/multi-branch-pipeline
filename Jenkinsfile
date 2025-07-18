 pipeline {
    agent {
        label 'java-slave'
    }
    environment{
        name = 'siva'
        roll no = '26'
    }
    stages{
        stage('build'){
            environment{
                class = 'mca'
            }
            steps{
                echo "my name is ${name}"
                echo "my roll no is ${roll no}"
                echo "class : ${class}"
            }
        }
    }
}
