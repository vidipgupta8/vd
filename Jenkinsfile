pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Hello1') {
            steps {
                echo 'Hello World1'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'hello', subject: 'hello', to: 'vidipgupta@gmail.com'
        }
    }
}
