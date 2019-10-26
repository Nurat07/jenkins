pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hi tarun'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'this is test branch'
          }
        }
        stage('test2') {
          steps {
            sh '''#!/bin/bash
echo "this is parallel branch"'''
          }
        }
      }
    }
  }
}