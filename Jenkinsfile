pipeline {
    agent any
    stages {
        stage('Ansible-playbook') {
            steps {
                // ansiblePlaybook(credentialsId: 'dummy', inventory: 'ansible/inventory', playbook: 'ansible/playbook.yaml')
                sh '''
                ansible-playbook -i ansible/inventory --user fmuyassarov ansible/playbook.yaml
                '''
            }
        }
    }
}
