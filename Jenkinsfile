pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        sh '''grep -q \'^user:\' /etc/passwd && echo "1" > /tmp/user || echo "0" > /tmp/user
'''
      }
    }

  }
}