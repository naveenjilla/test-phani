pipeline {
  agent {
    label "master"
  }

  stages {
    stage('clone') {
      steps {
        script {
          echo "checking out source code"
          checkout scm
        }
      }
    }

    stage('login') {
      steps {
        script {
          // sh " "
          echo "this is login stage"
        }
      }
    }

    stage('publish') {
      steps {
        script {
          // sh " "
          echo "this is publish stage"
        }
      }
    }

    stage('logout') {
      steps {
        script {
          // sh " "
          echo "this is logout stage"
        }
      }
    }
  }
}
