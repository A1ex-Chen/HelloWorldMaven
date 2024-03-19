pipeline {
  agent any
  tools { 
      maven 'M2_HOME' 
      jdk 'JAVA_HOME_8' 
  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/A1ex-Chen/HelloWorldMaven.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}
