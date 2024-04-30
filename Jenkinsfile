pipeline{
    agent any
    stages{
        stage('Branch test'){
            steps{
                echo "the branch name is ${env.BRANCH_NAME}"
            }
        }
        stage('cat README'){
            when{
                branch "UAT"
            }
            steps{
                sh '''
                cat README.md
                '''
            }
        }
    }
}
