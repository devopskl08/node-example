pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        DEPLY_TO = "development"
    }
    stages{
        stage('prodenv'){
            when {
               environment  name:'DEPLY_TO', value:'production'
            }
            steps{
              echo "deply to prod"
            }
        }
    }
}
