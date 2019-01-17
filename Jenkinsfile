node{
  gradle4 = tool 'gradle4'
  stage('checkout'){
        checkout scm
      }
  stage ('build'){
      sh "${gradle4}/bin/gradle jar"
      }
  stage ('archive'){
      archiveArtifacts artifacts: '**/build/libs/*.jar', fingerprint: true
      }
  }
