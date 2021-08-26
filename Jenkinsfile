pipeline {
    agent any
    stages {

        stage("Build")
        {
            steps
            {
                nodejs(cacheLocationStrategy: workspace(), nodeJSInstallationName: 'node-lts') {
                sh 'npm install'
                }
            }
        }

        stage("Unit Tests")
        {
            steps
            {
                nodejs(cacheLocationStrategy: workspace(), nodeJSInstallationName: 'node-lts') {
                sh 'npm run test:unit'
                }
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
