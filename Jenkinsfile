
pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        course = "kubernetes"
        GITHUB_CRED = credentials('hanu_ssh_cred')
    }
    stages{
        stage('first stage'){
            steps{
    
                echo "welcome to git hub account ${GITHUB_CRED}"
                echo "username ${GITHUB_CRED_USR}"
                echo "password is ${GITHUB_CRED_PSW}"
            }
        }
    }
}
