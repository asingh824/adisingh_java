@Library('my-shared-library') _
pipeline{
    agent any
    tools {
        maven 'mvn'
    }
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
        stage('Unit Test maven'){
        when { expression {  params.action == 'create' } }
            steps{
                script{

                    mvnTest()
                    
                }
            }
        }
        stage('Maven Int Test'){
            steps{
                script{

                    mvnIntegrationTest()
                    
                }
            }
        }

    }
}