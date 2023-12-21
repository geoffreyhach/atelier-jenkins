pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        sh '''sh \'grep -q "^user:" /etc/passwd > /tmp/user\'
sh \'/tmp/user\'
'''
      }
    }

  }
}