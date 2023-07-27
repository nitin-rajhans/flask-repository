pipeline {
    agent any
    stagess {
        stage('scm checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/nitin-rajhans/flask-repository.git'    
            }
            
        }
        stage ('docker image build'){
            steps {
                sh '/usr/bin/docker image build -t nitin0605/pipeimage . '
            }    
        }
    }
}
