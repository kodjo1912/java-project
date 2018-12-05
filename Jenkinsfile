pipeline {
    agent none
    tools {
        ant 'ant-1.10.5'
    }
    stages {
        
        stage('Run tests') {    
            agent any
            steps {
                sh 'ant -f test.xml -v'
            }
        }
        stage('Build') {    
            agent any
            steps {
                sh 'ant -f build.xml -v'
            }
        }
        
    }
}
