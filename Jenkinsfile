pipeline{
	agent any
	stages{
		stage ( 'Build' ) {
                    steps{
                      sh  'sleep 5 ; echo "This is Build" '
                         }
                                  }
		stage ( 'Test' ) {
		     steps{
                       sh ''' sleep 10
			     echo "This is Test phase" '''  
			  }	
                                 }
		stage ( 'Deploy' ){
		      steps{
			sh ''' sleep 10
		 	      echo "This is Deploy Phase" ''' 
   			   }			
	 			  }

              }

        }
