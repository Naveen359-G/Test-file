pipeline {
  agent any
  
  stages {
    stage ('Compile Stage') {
      
      steps {
        withMaven(maven : 'maven3') {
          sh 'mvn clean compile'
        }
      }
    }
    stages {
    stage ('Testing Stage') {
      
      steps {
        withMaven(maven : 'maven3') {
          sh 'mvn clean test'
        }
      }
    }
      
      stages {
    stage ('Deployment Stage') {
      
      steps {
        withMaven(maven : 'maven3') {
          sh 'mvn clean deploy'
        }
      }
    }
      }
    }
  }
