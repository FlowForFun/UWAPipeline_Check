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
        bat(script: 'svn up E:\\AntMan_android_dev', encoding: 'gb2312', label: '123', returnStatus: false, returnStdout: false)
      }
    }

    stage('CheckResource') {
      agent {
        node {
          label 'Local'
        }

      }
      steps {
        bat(script: 'curl -H "Content-Type:application/json" -X POST -d "{\\"exePath\\":\\"D:\\\\UwaProjScan\\\\UwaDataUploader\\\\LOCALService.exe\\",\\"unityPath\\":\\"RDpcUHJvZ3JhbSBGaWxlc1xVbml0eTIwMTguNC4yNmYxXEVkaXRvclxVbml0eS5leGU=\\",\\"projectPath\\":\\"RTpcQW50TWFuX2FuZHJvaWRfZGV2\\",\\"projectName\\":\\"QW50TWFuQW5kcm9pZERldg==\\",\\"type\\":\\"LOCALUPLOAD\\",\\"buildId\\":\\"%BUILD_ID%\\",\\"pipelineName\\":\\"Q2hlY2tSZXNvdXJjZQ==\\",\\"branchName\\":\\"bWFpbg==\\",\\"computerType\\":\\"MQ==\\"}" http://localhost:9898', encoding: '', label: '', returnStatus: '', returnStdout: '')
      }
    }

  }
}