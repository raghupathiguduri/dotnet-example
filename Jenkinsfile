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
    /*stage('Docker Build') {
      when {
        expression { params.BRANCH == 'develop' }
      }
      steps {
        withCredentials([usernamePassword(credentialsId: 'nexus', usernameVariable: 'username', passwordVariable: 'password')]) {
          DockerBuild(BUILD_NUMBER, username, password)
        }
      }
    }/*
  }
}
