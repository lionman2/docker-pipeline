pipeline {
  agent {any}
  stages {
     stage("Build Docker"){
      steps{
        docker.build("Dockerfile")
      }
    }
    stage("Run docker") {
      steps {
        docker.inside(){
           sh "whoami"
         }
     }
   }
}
