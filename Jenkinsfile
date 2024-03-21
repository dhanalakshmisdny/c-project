pipeline {
  agent any
  stages {
    stage("Clone Repo"){
      steps{
        sh 'rm -rf /var/lib/jenkins/workspace/test/c-project'
        sh 'git clone https://github.com/dhanalakshmisdny/c-project.git'
      }
    }
    stage("Build project"){
      steps {
        sh 'gcc test.c -o app'
      }
    }
  }
}
