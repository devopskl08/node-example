pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        DEPLY_TO = "development"
    }
    stages{
        stage('prodenv'){
            when{
                DEPLY_TO = "production"
            }
            steps{
              echo "deply to prod"
            }
        }
    }
}
