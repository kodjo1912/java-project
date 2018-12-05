pipeline {
    agent none
    tools {
        ant 'ant-1.10.5'
    }
    stages {
        stage('Example Build') {    
            agent any
            steps {
                sh 'ant -f test.xml -v'
            }
        }
    }
}
