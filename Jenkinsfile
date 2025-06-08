pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
                script{
                    echo "Checking out the code from SCM"
                    checkout scm
                }
            }
        }
    }
}