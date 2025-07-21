 pipeline{
    agent {
        label 'java-slave'
    }
    stages{
        stage('build'){
            steps{
                echo " build success "
            }
        }
        stage('test'){
            steps{
                echo 'test success'
            }
        }
        stage('Docker build'){
            steps{
                echo 'Docker build success'
            }
        }
        stage('Dev deploy'){
            steps{
                echo "devdeploy success"
            }
        }
        stage('Test deploy'){
            steps{
                echo " Test deploy success"
            }
        }
        stage('Stage deploy'){
            when {
                branch 'release-*'
            }
            steps{
                echo "Stage deploy success"
            }
        }
        stage('Production deploy'){
            when{
                tag pattern: "v\\d{1,2}.\\d{1,2}.\\d{1,2}", comparator: "REGEXP"
            }
            steps{
                echo "production deploy success"
            }
        }
    }
}
