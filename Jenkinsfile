//gitOpsPipeline name: 'test',
//               type: 'gradlew'
//gitOpsTest()

pipeline {
  options { 
    disableConcurrentBuilds()
    buildDiscarder(logRotator(numToKeepStr: '10'))
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
