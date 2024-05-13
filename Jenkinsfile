pipeline{
 agent any
  stages{
  stage('BUILD') {
    steps{
    echo "This is Build stage"
     sh '''
      sleep 5
      exit 0
      '''
    }
  }
    stage('TEST PARALLELE') {
     parallel {
      stage ('TEST ON CHORME') {
      steps{
        echo "This is Test on Chrome Browser "
        sh 'sleep 5; exit 1'
      }
      }
      stage ('TEST ON SAFARI') {
      steps{
        echo "This is Test on Safari Browser "
        sh 'sleep 5; exit 1'
      }
      }
      }
    }
    stage('DEPLOY') {
     parallel {
      stage ('SERVER 1') {
      steps{
        echo "This is Deploy to Server 1"
        sh 'sleep 5'
      }
      }
      stage ('SERVER 2') {
      steps{
        echo "This is Deploy to Server 2"
        sh 'sleep 5'
      }
    }
      stage ('SERVER 3') {
      steps{
        echo "This is Deploy to Server 3"
        sh 'sleep 5'
      }
      }
      stage ('SERVER 4') {
      steps{
        echo "This is Deploy to Server 4"
        sh 'sleep 5'
      }
      }
  }
}
  }
}
