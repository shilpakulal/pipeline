pipeline{
 agent none
  stages{
  stage('BUILD') {
   agebt any
    steps{
    echo "This is Build stage"
      sh 'sleep 5'
    }
  }
    stage('TEST') {
     agent {label 'jenkins'}
      steps{
        echo "This is Test stage"
        sh 'sleep 5'
      }
    }
    stage('DEPLOY') {
     agent {label 'master'}
      steps{
        echo "This is Deploy stage"
        sh 'sleep 5'
      }
    }
  }
}
