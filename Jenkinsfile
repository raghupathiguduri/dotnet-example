@Library("jenkins-shared-library_raghu@main") _
pipeline {
    agent any
  stages {
    stage('Checkout') {
      steps {
        deleteDir()
        echo "Checking out....."
        checkout scm
      }
    }
    stage('Build App') {
      steps {
        Builddotnet()
      }
    }
  }
}
