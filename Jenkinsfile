pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/Kranti143/CTS.git', branch: 'master', credentialsId: 'Kranti143')
      }
    }
    stage('build') {
      steps {
        sh '''#!/bin/bash
mvn clean compile'''
      }
    }
  }
}