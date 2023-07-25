pipeline {
    agent any
    stages {
        stage('Print') {
            steps {
                // ansiblePlaybook(credentialsId: 'dummy', inventory: 'ansible/inventory', playbook: 'ansible/playbook.yaml')
                sh '''
                ls -lah
                pwd
                ls /var/jenkins_home/workspace/
                '''
            }
        }
        stage('Ansible-playbook') {
            steps {
                // ansiblePlaybook(credentialsId: 'dummy', inventory: 'ansible/inventory', playbook: 'ansible/playbook.yaml')
                sh '''
                ansible-playbook -i ansible/inventory --user fmuyassarov ansible/playbook.yaml -vvvv
                '''
            }
        }
    }
}
