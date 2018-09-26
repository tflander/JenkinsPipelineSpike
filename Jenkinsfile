pipeline {
  agent any
  stages {
    stage('Git Fetch') {
      steps {
        dir(path: 'rules') {
          git(branch: 'master', url: 'https://github.com/tflander/rulesEngineLambda.git')
        }

        dir(path: 'functionalKoans') {
          git(url: 'https://github.com/tflander/FunctionalRefactoringKoans.git', branch: 'master')
        }

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