pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG21CS368-1.cpp -o temp'
                 build job: 'PES1UG21CS368-1', wait: false
                 echo 'Build by CS368 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG21CS368-1.cpp'
                echo 'Test by CS368 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS368 successful'
            }
        }
    }

    post {
        failure {
           
                echo 'Pipeline Failed'
         
        }
    }
}
