pipeline{
 agent any 
  stages{
    stage ('Build'){
      steps {  
        echo 'running build'
       sh './gradle wrapper --gradle-version 7.2'
        sh './gradlew build no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
