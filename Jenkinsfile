pipeline {
  
  // use only nodes marked as 'tensorflow'
  agent { node { label 'tensorflow' } }
  
  stages {

  stage('Clone repository') {
        checkout scm
        }

    stage('Training') {
      steps {
        echo "Training problem"
            sh "python tf_example.py"
        echo "All done"
      }
    }
  }
}
