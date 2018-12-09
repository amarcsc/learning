node{
    //checkout
    echo "$BRANCH_NAME"
    echo env.BRANCH_NAME
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'amargit', url: 'https://github.com/amarcsc/learning.git']]])
    }
   
    
    //build
    stage('Build'){
         bat(/mvn  clean install/)
    
    }
}
