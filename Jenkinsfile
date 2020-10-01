pipeline {
    agent any
    stages {
        stage('SCM Integration') {
            steps {
                echo 'I am conencting with GitHub for source code'
                git 'https://github.com/pavansw/ab-inbevDevops.git'
            }
        }
        stage('Run Python code') {
            steps {
                echo 'I am Running Hello.py from source code'
                sh 'python hello.py'
            }
        }
        stage('Confirmation All Good') {
            steps {
                echo 'I am declairing that Pipeline is successful'
                sh 'echo "ALL GOOD"'
            }
        }
  }
}

