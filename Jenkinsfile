pipeline{
    agent any
    stages{
        stage('Git Checkout'){
            steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Reliable-Cloud-Services-LLC/base-docker-pipeline.git']]])
             
            }
        }
    stage('Build Python App'){
        steps{
            sh '''cd Python-3-image
        docker build -t python .
        '''
        }
    }

    stage('Build Java App'){
      steps{
         sh '''cd Java-11-image
    docker build -t java .
    '''

      }
    }






    }
}
