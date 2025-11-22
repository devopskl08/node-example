
pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        course = "kubernetes"
        name = "likhitha"
        cloud = "AWS"
    }
    stages{
        stage('first stage'){
            environment {
                cloud = "gcp"
            }
            steps{
                echo "helllo  ${name}!!"
                echo "welcome to ${course}. All the best ${name}"
                echo "welcome to ${cloud}"
            }
        }
        stage('second stage){
              steps{
                   echo "helllo  ${name}!!"
                echo "welcome to ${course}. All the best ${name}"
                echo "welcome to ${cloud}"
            }
        }
    }
}
