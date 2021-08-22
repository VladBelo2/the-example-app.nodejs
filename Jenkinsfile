pipeline {
    agent any
    stages {

        stage("Build")
        {
            steps
            {
                sh 'npm install'
            }
        }

        stage("Unit Tests")
        {
            steps
            {
                sh 'npm run test:unit'
            }
        }

        stage("Upload Artifacts")
        {
            steps
            {
                echo "skip"
            }
        }

        stage("Deploy to Dev Env")
        {
            steps
            {
                echo "skip"
            }
        }
    }
}
