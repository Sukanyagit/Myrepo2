node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Sukanyagit/MyRepo2.git']]])
    }
    stage('Testing')
    {
        sh label: '', script: 'mvn test'
    }
    stage('Packaging')
    {
        sh label: '', script: 'mvn package'
    }
}
