@Library('my-shared-library1') _
pipeline{
    agent any

    stages{
        stage('Git Checkout'){
            steps{
                script{

                    gitCheckout(
                        branch: "main",
                        url: "https://github.com/asingh824/adisingh_java.git"
                    )
                    
                }
            }
        }  
    }
}