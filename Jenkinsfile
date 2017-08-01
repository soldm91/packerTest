pipeline {
  agent any
  stages {
    stage('Test Packer') {
      steps {
        echo 'Testing Packer'
        sh '''(cd /var/lib/jenkins/terraformPractice/; sudo git pull)
cp -f /var/lib/jenkins/variables/variables.json variables.json
cp -f /var/lib/jenkins/terraformPractice/rhel.json rhel.json
cp -f /var/lib/jenkins/terraformPractice/script.sh script.sh
cp -f /var/lib/jenkins/terraformPractice/hello.txt hello.txt
packer --version'''
      }
    }
  }
}