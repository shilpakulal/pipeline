pipeline{
  agent any;
  stages{
  stage('BUILD') {
    steps{
    echo "This is Build stage"
    }
  }
    stages('TEST') {
      steps{
        echo "This is Test stage"
      }
    }
    stages('DEPLOY') {
      steps{
        echo "This is Deploy stage"
      }
    }
  }
}
