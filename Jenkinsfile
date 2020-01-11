node {
    def app

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }
    stage('Java build') {
        sh "mvn clean install"
    }
    stage('Deployment in server') {
        sh "ansible-playbook java.yml"
    }
}
