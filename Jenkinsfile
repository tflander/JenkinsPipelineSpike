pipeline {
  agent any
  stages {
    stage('Git Fetch') {
      steps {
        git(url: 'https://github.com/tflander/FunctionalRefactoringKoans.git', branch: 'master')
        git(url: 'https://github.com/tflander/rulesEngineLambda.git', branch: 'master')
      }
    }
  }
}