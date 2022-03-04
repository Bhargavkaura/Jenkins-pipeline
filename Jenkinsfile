pipeline{
	agent none
	stages{
	   stage ( 'Build' ) {
	   agent { label 'node1'}
                    steps{
                      sh  'sleep 5 ; echo "This is Build" '
                         }                
                }
	    
   		stage ( 'Test' ) {
		agent { label 'master'}
		     steps{
                       sh ''' sleep 10
			     echo "This is Test phase" '''  
			  }	
                                 }
		stage ( 'Deploy' ){
		agent { label 'node1'}
		      steps{
			sh ''' sleep 10
		 	      echo "This is Deploy Phase" ''' 
   			   }			
	 			  }

              }

        }
