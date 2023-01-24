pipeline {
    agent any 
  stages {
        stage(' Ansible Execution') {
            steps {
              ansiblePlaybook credentialsId: '43.207.48.0', disableHostKeyChecking: true, installation: 'ansible', inventory: 'ansible.inv', playbook: 'ansible.yml' 
            }
        }
    }
}
