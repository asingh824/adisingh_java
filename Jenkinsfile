
pipeline{
    agent any

    stages{
        stage('Git Checkout'){
            steps{
                script{

                    gitCheckout(
                        git branch: "main"
                        url: "https://github.com/asingh824/adisingh_java.git"
                    )
                    
                }
            }
        }  
    }
}