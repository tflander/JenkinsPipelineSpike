pipeline {
  agent any
  stages {
    stage('Git Fetch') {
      steps {
        sh '''mkdir refactoring
cd refactoring
'''
        git(url: 'https://github.com/tflander/FunctionalRefactoringKoans.git', branch: 'master')
        sh '''cd ..
mkdir rules
cd rules
'''
        git(url: 'https://github.com/tflander/rulesEngineLambda.git', branch: 'master')
      }
    }
    stage('Show Workspace') {
      steps {
        sh '''pwd
ls -lrt'''
      }
    }
  }
}