pipeline {

  agent any

  stages {
    stage('Checkout') {
      steps {
          git branch: 'main', url: 'https://github.com/iamsr16/dotnet-app.git'
          }
     }
    stage('Restore packages') {
      steps {
        dotnet restore
      }
    }

    stage('Build') {
      steps {
        dotnet build
       }    
    }
  }
}
