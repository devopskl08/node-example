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
            when {
                expression{
                    BRANCH_NAME ==~  /(production|staging)/
                }
            }
            steps{
                echo "deplying to stage"
            }
        }

        stage('deplytoprod'){
            when {
                expression{
                    BRANCH_NAME ==~  /(production|staging)/
                }
            }
            steps{
                echo "deplying to prod"
            }
        }
    }
}
}
