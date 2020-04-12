pipeline {
    agent {label 'master'}
    stages {
        stage("Windows Shutdown") {
        steps {
            sh "export ANSIBLE_HOST_KEY_CHECKING=False && ansible-playbook -i inventory.ini shutdown.yml"
        }
    }
  }
}
