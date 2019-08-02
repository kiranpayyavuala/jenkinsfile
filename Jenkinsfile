pipeline {
    agent any

    stages {
        stage ('Build Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean install'
                }
            }
        }
    stage('Build Docker Image')
   {
   sh 'docker build -t kiranpayyavuala/myapp:1.0 .'
    }
  }
}
