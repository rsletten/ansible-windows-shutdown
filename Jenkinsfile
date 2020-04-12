pipeline {
    agent {label 'master'}
    stages {
        stage("Windows Shutdown") {
        steps {
            sh "export ANSIBLE_HOST_KEY_CHECKING=False && ansible-playbook -i /var/jenkins_home/ansible/ansible-windows-shutdown/inventory.ini /var/jenkins_home/ansible/ansible-windows-shutdown/shutdown.yml"
        }
    }
  }
}
