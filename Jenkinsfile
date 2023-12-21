pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        sh '''grep -q \'^user:\' /etc/passwd && echo "1" > /tmp/user || echo "0" > /tmp/user
cat /etc/passwd'''
      }
    }

    stage('step 2') {
      steps {
        sh '''if grep -q "0" /tmp/user; then
    find / -user user
else
    echo "user n\'existe pas."
fi'''
      }
    }

  }
}