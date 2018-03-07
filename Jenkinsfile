node('tensorflow')
{
  stage('Clone repository') {
        git url: "https://github.com/abhisheksurendran14/GitRepository.git", credentialsId: 'abhisheksurendran14'
        checkout scm
        }
  stage('Prepare'){
     sh '''
   pip install tensorflow 
   '''
  }

    stage('Training') {
        echo "Training problem"
            sh "python tf_example.py"
        echo "All done"
    }
}
