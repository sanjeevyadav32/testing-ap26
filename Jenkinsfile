pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/sanjeevyadav32/testing-ap26.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building project..."
                sh 'echo Hello from Jenkins Pipeline 🚀'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'echo Tests passed ✅'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy step..."
                sh 'echo Deployment done 🎉'
            }
        }
    }
}
