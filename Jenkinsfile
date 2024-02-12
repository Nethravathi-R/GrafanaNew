pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf GrafanaNew'
        sh 'git clone https://github.com/Nethravathi-R/GrafanaNew.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana.yml'
      }
    }
  }
}
