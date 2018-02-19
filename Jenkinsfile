pipeline {
  agent any
  stages {
    stage('RunVBS_A') {
      steps {
        bat(script: 'Wscript "C:\\Devaraj\\Test\\a.vbs"', returnStatus: true, returnStdout: true)
      }
    }
  }
}