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
        stage('Deploy') {    
            agent any
            steps {
                sh 'aws s3 cp /workspace/Java-pipeline/dist/rectangle-${BUILD_NUMBER}.jar s3://kodjo-seis665-02-fall2018'
            }
        }
        
    }
}
