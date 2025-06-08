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
        stage("Build") {
            steps {
                script {
                    echo "Building the project"
                    sh 'echo "Building the project..."'
                    sh 'pwd'
                    sh 'ls'
                    sh 'python3 -m venv myenv'
                    sh 'source myenv/bin/activate && pip install -r requirements.txt'
                    sh 'source myenv/bin/activate && python streamlit run app'

                }
            }
        }
    }
}