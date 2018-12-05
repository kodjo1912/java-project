pipeline {
    agent none
    tools {
        ant 'ant-1.10.5'
    }
    stages {
        stage('Example Build') {            
            steps {
                sh 'ant -f test.xml -v'
            }
        }
    }
}
