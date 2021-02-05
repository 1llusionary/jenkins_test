pipeline {
    agent { label 'spider' }

    stages {
        stage('Pull Code') {
            steps {
                git branch: 'main', url: 'https://github.com/1llusionary/jenkins_test.git'
            }
        }
        stage('Run') {
            steps {
                sh 'python2 hello_world.py'
            }
        }
    }
}
