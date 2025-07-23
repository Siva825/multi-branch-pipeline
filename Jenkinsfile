 pipeline{
    agent any
    parameters{
        string(name:'Application',description:'',defaultValue:'Devops')
        booleanParam(name:'RUN_TESTS', description:'would you like to run tests',defaultValue:true)
        choice(name:'Env_name',description:'',choices:['dev', 'test', 'prod'])
        password(name:'Password',description:'Enter your password here',defaultValue:'secretpassword')
    }
    stages{
        stage('Build'){
            steps{
                echo "build is ongoing"
                echo "${params.Application}"
                echo "${params.RUN_TESTS}"
                echo "${params.Env_name}"
                echo "${params.Password}"

            }
        }
    }
}
