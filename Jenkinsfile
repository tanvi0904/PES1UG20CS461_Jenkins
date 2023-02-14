pipeline
{
    agent any
    stages
    {
        stage('Build')
        {
            steps
            {
                echo 'Building...'
                sh 'g++ pes1ug20cs461_hello.cpp'
                sh '/var/jenkins_home/workspace/pes1ug20cs461-1/main/hello_exec'
            }
        }
        stage('Test')
        {
            steps
            {
                echo 'Testing...'
                sh './a.out'
            }
        }
        stage('Deploy')
        {
            steps
            {
                echo 'Deploying...'
            }
        }
    }
    post
    {
        failure
        {
            echo 'Pipeline Failed'
        }
    }
}