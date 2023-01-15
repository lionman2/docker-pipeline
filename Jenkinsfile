pipeline {
  agent any
  stages {
     stage("Build Docker"){
      steps{
        docker.build("Dockerfile")
      } //steps
     } //stage
     stage("Run docker") {
       steps {
         script {
           docker.inside(){
            sh "whoami"
          } //docker
         } //script
       } //steps
     }//stage
   } //stages
}//pipeline
