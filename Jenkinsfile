@Library('shared-library') _

pipeline{

    agent any

    stages{
    stage('git checkout'){

    steps{

       script{

             gitCheckout(
                  
		  branch: "master",
		  url: "https://github.com/veeresh595/JavaCICDapp.git"

                   )
       }
      }

       stage('Unit testing'){

         steps{
	      
	      scripts{

	            mvnTest()

        }
       }
      }
     }
    }
   } 
