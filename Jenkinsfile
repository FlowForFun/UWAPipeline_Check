pipeline {
  agent any
  stages {
    stage('do batch') {
      agent {
        node {
          label 'Local'
        }

      }
      steps {
        bat(script: 'svn up E:\\AntManAndroidDev', encoding: 'gb2312', label: '123', returnStatus: false, returnStdout: false)
      }
    }

  }
}