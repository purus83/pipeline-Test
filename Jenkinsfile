pipeline {
    agent { node { label 'master' } }
    stages {
        stage('First-Step'){
            steps {
                sh 'cat /etc/fstab'
                }
        }
    }
}
