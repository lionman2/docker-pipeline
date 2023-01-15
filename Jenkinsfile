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
        docker.inside(){
           sh "whoami"
         } //docker
       } //steps
     }//stage
   } //stages
}//pipeline
