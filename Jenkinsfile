pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        course = "kubernetes"
        name = "likhitha"
    }
    stages{
        stage('first stage'){
            steps{
                echo "helllo  ${name}!!"
                echo "welcome to ${course}. All the best ${name}"
            }
        }
    }
}
