pipeline {
    agent any
	

 stages {
      stage('checkout') {
           steps {
             
                git branch: 'main', url: 'https://github.com/thhr53/centralrepo.git'
             
          }
        }
       

  stage('Docker Build and Tag') {
           steps {
              
                sh 'docker build -t devopsclass:latest .' 
                sh 'docker tag devopsclass srikanta1219/devopsclass:$BUILD_NUMBER'
               
          }
        } 
    }
}
