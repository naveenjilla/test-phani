pipeline {
  agent {
    label "master"
  }

  parameters {
    choice(name: 'server', choices: ['server1', 'server2', 'server3'], description: '')
    string(name: 'USERNAME', defaultValue: 'xyz', description: '')
    password(name: 'PASSWORD', description: 'password')
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
          sh "apic-slim.exe login --server ${server} --realm provider/default-idp-2 --username ${USERNAME} --password ${PASSWORD} --accept-license  "
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
