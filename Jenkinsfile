#!/usr/bin/env groovy

pipeline {
  options {
    timestamps()
    skipDefaultCheckout()
  }
  environment {
    ONE=1

  }
  agent any
  stages {
    stage ('run Playbook...'){
      steps {
        script {
          powershell(returnStdout: true, script: "cygwin ansible")

          // ansiblePlaybook(
          // playbook: 'ping.yml',
          // inventory: 'hosts'
          // )
        }

      }
    }
  }
}
