pipeline{
    agent{
        label 'slave-1'
    }
    stages{
        stage('build'){
            steps{
                echo "building applicayion"
            }
        }
        stage('scans'){
            steps{
                echo "scans performing"
            }
        }
        stage('deplytodev'){
            steps{
                echo "deplying to dev"
            }
        }
        stage('deplytotest'){
            steps{
                echo "deplying to test"
            }
        }
        stage('deplytostage'){
            steps{
                echo "deplying to stage"
            }
        }

        stage('deplytoprod'){
            steps{
                echo "deplying to prod"
            }
        }
    }
}
