pipeline 
{
    agent any

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Test Application'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploy Aplication'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Build Status in detail avaialble at the Jenkins site', subject: 'Build Status', to: 'cinuts10@gmail.com'
        }
    }
}
