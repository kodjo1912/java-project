pipeline {
    agent none
    tools {
        ant 'ant-1.9.6'
    }
    stages {
        stage('test ant exists') {
            steps {
                sh 'ant -v'
            }
        }
        stage('Example Build') {            
            steps {
                sh 'ant -f test.xml -v'
            }
        }
    }
}
