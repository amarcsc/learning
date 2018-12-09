node{
    //checkout
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: 'feature/jira-001']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'amargit', url: 'https://github.com/amarcsc/learning.git']]])
    }
   
    
    //build
    stage('Build'){
         bat(/mvn  clean install/)
    
    }
}
