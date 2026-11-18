pipeline{
    agent any

    stages{
        stage("build"){
            steps{
                echo "Building an Application"
                echo "So the current branch is ${env.BRANCH_NAME}"
            }
        }
        stage("develop"){
            when {
                branch "development"
            }
            steps{
                echo "This is a development environment"
            }

        }
        stage("testing"){
            when{
                branch "testing"
            }
            steps{
                echo "This is testing environment"
            }
        }
        stage("feature")
        {
            when{
                branch "feature/login"
            }
            steps{
                echo "This is a feature branch"
            }
        }
        stage("Final"){
            when{
                branch "production"
            }
            steps{
                echo "THis is a production environment"
            }
        }
    }
}