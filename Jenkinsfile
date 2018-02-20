pipeline {
  agent any
  stages {
    stage('RunVBS_A') {
      steps {
        parallel(
          "RunVBS_A": {
            bat(script: 'Wscript "C:\\Devaraj\\Test\\a.vbs"', returnStatus: true, returnStdout: true)
            
          },
          "RunVBS_B": {
            bat(script: 'Wscript "C:\\Devaraj\\Test\\b.vbs"', returnStatus: true, returnStdout: true)
            
          },
          "RunVBS_C": {
            bat(script: 'WScript "C:\\Devaraj\\Test\\c.vbs"', returnStatus: true, returnStdout: true)
            
          }
        )
      }
    }
    stage('RunVBS_D') {
      steps {
        parallel(
          "RunVBS_D": {
            bat(script: 'WScript "C:\\Devaraj\\Test\\d.vbs"', returnStatus: true, returnStdout: true)
            
          },
          "RunVBS_E": {
            bat(script: 'WScript "C:\\Devaraj\\Test\\e.vbs"', returnStatus: true, returnStdout: true)
            
          }
        )
      }
    }
  }
}