#!/usr/bin/env groovy

pipeline {
  options {
    timestamps()
    skipDefaultCheckout()
  }
  environment {

  }
  agent any
  stages {
    stage ('run Playbook...'){
      steps {
        script {
          bat ("pwd")
          ansiblePlaybook(
          playbook: 'ping.yml',
          inventory: 'hosts'
          )
        }
        
      }
    }
  }
}
