pipeline {
    agent any 
    stages {
        stage('Build System Details') {
            steps {
                // Fixed the missing quote and aligned the multi-line block
                sh '''
                    echo "System Details:"
                    uname -a
                '''
            }
        }
        stage('Memory') {
            steps {
                sh '''
                    echo "Memory details:"
                    free -h
                '''
            }
        }
        stage('CPU Details') {
            steps {
                sh '''
                    echo "CPU details:"
                    lscpu
                '''
            }
        }
        stage('Date') {
            steps {
                sh '''
                    echo "Current Date and Time:"
                    date
                '''
            }
        }
        stage('current process') {
            steps {
                sh '''
                echo "current process"
                ps -eaf | head
                '''
            }
        }
        stage('hostname') {
            steps {
                sh '''
                echo "hostname"
                hostname
                '''
            }
        }
    }
}
