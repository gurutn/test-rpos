pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        httpRequest(url: 'http://urda:8080/job/RC-9.4/lastSuccessfulBuild/api/json?', acceptType: 'APPLICATION_JSON', contentType: 'APPLICATION_JSON', httpMode: 'GET', ignoreSslErrors: true, outputFile: 'lastsuccessfulBuild.txt', validResponseCodes: '200', responseHandle: 'STRING')
      }
    }

  }
  environment {
    temp = ''
  }
}