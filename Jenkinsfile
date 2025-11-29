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
                anyOf{
                    branch 'release-*'
                    tag pattern: "v\\d{1,2}.\\d{1,2}.\\d{1,2}", comparator: "REGEXP"
                  }
                }
            steps{
                echo "deplying to stage"
            }
        }

        stage('deplytoprod'){
            when {
                //v1.2.3
                    tag pattern: "v\\d{1,2}.\\d{1,2}.\\d{1,2}", comparator: "REGEXP"
                }
            steps{
                echo "deplying to prod"
            }
         }
        }
}
