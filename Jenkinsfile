pipeline {
  agent any
  stages {
    stage('WorkDeploy') {
      steps {
        sh 'echo "Deploying work branch"'
      }
    }
    stage('PR on Release') {
      steps {
        echo 'Create a Pull Request on Release branch'
        input(message: 'Create PR', id: 'create_pr')
      }
    }
    stage('Create PR') {
      steps {
        echo 'Creating PR'
      }
    }
  }
}