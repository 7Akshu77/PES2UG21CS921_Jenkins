pipeline{
  agent any 
  stages {
     jgmhhj stage('Clone repository'){
      //  steps{
      //  checkout([$class: 'GitSCM',
       //branches:[[name:'*/main']],
        //userRemoteConfigs :[[url:'https://github.com/7Akshu77/PES2UG21CS921_Jenkins.git']]])
   //}
   //}
    stage('Build'){
      steps{
       sh 'g++ hello.cpp -o output'
      }
    }
    stage('Test'){
      steps {
        sh './output'
      }
    }
    stage('Deploy'){
      steps{
        echo 'deploy'
      }
    }
  }
  post{
    failure{
      error 'Pipeline failed'
    }
  }
}
