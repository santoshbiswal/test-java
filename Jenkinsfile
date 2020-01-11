node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }
    stage('Run ansible playbook to configure nginx') {
        sh "mvn clean install"
    }
    stage('Run ansible playbook to configure nginx') {
        sh "ansible-playbook java.yml"
}
