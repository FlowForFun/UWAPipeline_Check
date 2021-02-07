pipeline {
  agent any
  stages {
    stage('do batch') {
      steps {
        bat(script: 'C:\\Windows\\ServiceProfiles\\LocalService\\.jenkins\\workspace\\Test_Build_main\\UpdateAntman.bat', encoding: 'gb2312', label: '123', returnStatus: false, returnStdout: false)
      }
    }

  }
}