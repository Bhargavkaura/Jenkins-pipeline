pipeline{
	agent none
	stages{
	  agent { label 'node1' }
		stage ( 'Build' ) {
                    steps{
                      sh  'sleep 5 ; echo "This is Build" '
                         }                
                }
	   agent { label 'master' }	
		stage ( 'Test' ) {
		     steps{
                       sh ''' sleep 10
			     echo "This is Test phase" '''  
			  }	
                                 }
	    agent { label 'node1' }
		stage ( 'Deploy' ){
		      steps{
			sh ''' sleep 10
		 	      echo "This is Deploy Phase" ''' 
   			   }			
	 			  }

              }

        }
