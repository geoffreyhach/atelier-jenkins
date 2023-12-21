pipeline {
  agent any
  stages {
    stage('step 1') {
      steps {
        sh '''grep -q \'^user:\' /etc/passwd && echo "1" > /tmp/user || echo "0" > /tmp/user
'''
      }
    }

    stage('') {
      steps {
        sh '''if grep -q "0" /tmp/user; then
    echo "Le fichier /tmp/user contient \'0\'."
else
    echo "Le fichier /tmp/user ne contient pas \'0\'."
fi'''
      }
    }

  }
}