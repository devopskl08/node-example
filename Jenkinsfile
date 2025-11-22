
pipeline{
    agent{
        label 'slave-1'
    }
    environment{
        course = "kubernetes"
        github_cred = credentials('hanu_ssh_cred')
    }
    stages{
        stage('first stage'){
            steps{
        
                echo "welcome to ${course}. All the best ${name}"
                echo "welcome to git hub account ${github_cred}"
                echo "username ${github_cred_USR}"
                echo "password is ${github_cred_USR_PSW}"
            }
        }
    }
}
