pipeline {
    agent any

    stages {
        stage('git') {
            steps {
                git 'https://github.com/Sannidhi10/Amazon-Clone-ansible.git'
            }
        }
        stage('ansible-deploy') {
            steps {
               bat 'ansible-playbook -i ./ansible/inventory ./ansible/ansible-playbook.yaml'
            }
        }
    }
}
