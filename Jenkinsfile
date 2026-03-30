pipeline{
  agent any
  stages{
    stage('checkout'){
      steps{
        git 'https://github.com/Ravi-Teja-S/Sundown-studio/'
      }
    }
    stage('build'){
      steps{
        sh 'echo "Building"'
    }
  }
    stage('test'){
      steps{
        sh'echo "Testing"'
    }
    }
      stage('deploy'){
        steps{
          sh 'echo "Deploying"'
      }
      }
  }

  post{
    success{
      sh 'echo "BUILD SUCCESSFUL" '
    }
    failure{
      sh 'echo "BUILD FAILED" '
  }
}
}
