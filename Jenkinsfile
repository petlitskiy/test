//gitOpsPipeline name: 'test',
//               type: 'gradlew'
//gitOpsTest()

pipeline {
  options { 
    disableConcurrentBuilds()
    buildDiscarder(logRotator(numToKeepStr: '10'))
  }
  triggers {
    issueCommentTrigger(issueTriggers)
    pullRequestReview(reviewStates: ['approved'])
  }
  agent any
  stages {
    stage('test') {
      steps {
        println ("It's alive!")
      }
    }
  }
}
