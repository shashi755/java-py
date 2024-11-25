pipeline {
    agent any

    stages {
        stage('Job 1: Clone Git Repository') {
            steps {
                script {
                    echo 'Cloning the GitHub repository...'
                    git branch: 'main', url: 'https://github.com/your-username/your-repository.git'
                }
            }
        }

        stage('Job 2: Execute Java Program') {
            steps {
                script {
                    echo 'Compiling and running the Java program...'
                    // Compile and run Java program
                    bat 'javac HelloWorld.java'
                    bat 'java HelloWorld'
                }
            }
        }

        stage('Job 3: Execute Python Program') {
            steps {
                script {
                    echo 'Running the Python program...'
                    // Execute Python script
                    bat 'python script.py'
                }
            }
        }
    }
}
