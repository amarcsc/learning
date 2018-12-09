node{
    //checkout
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'amargit', url: 'https://github.com/amarcsc/learning.git']]])
    }
   
    
    //build
    stage('Build'){
         bat(/mvn  clean install/)
    
    }
}
