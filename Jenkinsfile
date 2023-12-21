pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        sh '''grep -q \'^user:\' /etc/passwd > /tmp/user
cat /tmp/user
'''
      }
    }

  }
}