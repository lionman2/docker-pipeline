pipeline {
  agent any
  stages {
     stage("Build Docker"){
      steps{
        script {
          docker.build("myImage:${BUILD_ID}")
        }
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
