@Library('my-shared-library') _
pipeline{
    agent any

    stages{
        stage('Git Checkout'){
            steps{
                gitCheckout(
                    branch: 'main',
                    url: "https://github.com/asingh824/adisingh_java.git"
                )
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
    }
}