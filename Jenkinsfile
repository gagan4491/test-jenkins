pipeline {
    agent { label 'master' }
    
    parameters {
       extendedChoice(description: '', multiSelectDelimiter: ',', name: 'Masspay Test Suite', quoteValue: true, saveJSONParameterToFile: false, type: 'PT_CHECKBOX', value: 'Masspay-DEV,Masspay-SIT,Masspay-QA,Masspay-PROD', visibleItemCount: 4)    
      }
    stages {	
	    
	    stage('echo') {
		    steps {	    
		    
			   // echo "${params.Masspay-DEV}" 
		    }    
	    }
	    
               stage('build') {
            steps {
                cleanWs()
        }
                
                
        }
		
		}
		
		}
