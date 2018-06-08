pipeline {
  agent { label 'linux' }
  stages {
    stage('checkout'){
      steps{
        git 'https://github.com/fudanzz/spsdemo2.git'
      }
    }
    
    stage('build'){
      steps{
        sh 'mvn clean compile'
      }
    }
    
    stage('test'){
      steps{
        sh 'mvn  test'
      }
    }
    
    stage('package'){
      steps{
        sh 'mvn  package'
      }
    }
  
  }
}