pipeline {
    agent { node { label 'master' } }
    parameters { string(name:'TestString', defaultValue:'Default', description:'Test String') }
    stages {
        stage('First-Step'){
            steps {
                sh 'cat /etc/fstab'
                echo ${params.TestString}
                }
        }
    }
}
