my_image = ""
pipeline {
  agent any
  stages {
     stage("Build Docker"){
      steps{
        script {
          my_image = docker.build("myimage:${BUILD_ID}")
        }
      } //steps
     } //stage
     stage("Run docker") {
       steps {
         script {
           my_image.inside(){
            sh "echo 'lala'"
          } //docker
         } //script
       } //steps
     }//stage
   } //stages
}//pipeline
