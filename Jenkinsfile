pipeline {
    agent any stages {
        stage(' Ansible Execution') {
            steps {
              ansiblePlaybook credentialsId: 'ansible', disableHostKeyChecking: true, installation: 'ansible', inventory: 'ansible.inv', playbook: 'ansible.yml' 
            }
        }
    }
}
