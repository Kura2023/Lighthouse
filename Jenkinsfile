pipeline {
  agent {docker{ image 'node:8.12.0' }}
    environment {
        HOME = '.'
    }
  stages {
    stage('Git') {
      steps {
        git 'https://github.com/Kura2023/Lighthouse.git'
      }
    }
stage('Build') {
      steps {
         sh 'npm install'
         sh 'npm install puppeteer'
         sh 'node ./demo.js'
      }
    }  
 }
}
