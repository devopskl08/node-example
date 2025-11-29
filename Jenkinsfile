pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        DEPLY_TO = "development"
    }
    stages{
        stage('devenv'){
            steps{
                echo "deploy to dev env"
            }
        }
        stage('prodenv'){
            when{
                allOf{
                branch 'development'
                environment name: 'DEPLY_TO'  ,value: 'production'
            }
            steps{
              echo "deply to prod"
            }
        }
     }
}
}
