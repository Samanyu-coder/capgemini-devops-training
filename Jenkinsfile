pipeline {
    agent any

    stages {

        // stage('Checkout') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/Samanyu-coder/capgemini-devops-training.git'
        //     }
        // }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                if [ ! -d /Users/samanyudeghuria/Developer/log ]; then
                    mkdir -p /Users/samanyudeghuria/Developer/log
                fi

                cp index.html /Users/samanyudeghuria/Developer/log/
                '''
            }
        }
    }
}
