pipeline {
    agent { node { label 'master' } }
    parameters { string(name:'TestString', defaultValue:'Default', description:'Test String')
                 text(name:'Testtext', defaultValue:'DefaultText', description:'Test Text to check Text Parameter in Pipelines')
                 booleanParam(name:'TestBoolean',defaultValue:true, description:'Test Parameter to check Booplean Parameter')
                 choice(name:'TestChoice',choices:['left','right','straight'],description:'Test Parameter to check the choice Parameter')
                 password(name:'TestPAssword',defaultValue:'',description:'To test Password Parameter')
               }
    stages {
        stage('First-Step'){
            steps {
                sh 'cat /etc/fstab'
                echo "${params.TestString}"
                echo "${params.Testtext}"
                echo "${params.TestBoolean}"
                echo "${params.TestChoice}"
                echo "${params.TestPAssword}"
                }
        }
    }
}
