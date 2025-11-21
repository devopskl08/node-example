pipeline{
  agent{
    label 'slave-1'
  }
  tools{
    maven 'MAVEN_3.8.8'
  }
  stages{
    stage ("maven") {
      steps{
        echo "hello maven section"
        sh "mvn --version"
      }
    }
    stage ('second stage'){
      tools{
        maven 'MAVEN_3.9.6'
      }
      steps{
        echo "hello"
        sh "mvn --version"
      }
    }
  }
}
    
