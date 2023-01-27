pipeline {
  agent any
  environment {
    DOCKERHUB_CREDENTIALS = credentials('dockerHub')
  }
  stages {
   stage('Ansible')
    {
      steps{
          ansiblePlaybook credentialsId: '43.207.48.0', disableHostKeyChecking: true, installation: 'ansible', inventory: 'ansible.inv', playbook: 'rollback.yml'
      }
    }
  }
}
