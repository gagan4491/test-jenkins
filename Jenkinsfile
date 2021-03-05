pipeline {
    agent { label 'master' }
    
    parameters {
       extendedChoice(description: '', multiSelectDelimiter: ',', name: 'Masspay-Test-Suite', quoteValue: true, saveJSONParameterToFile: false, type: 'PT_CHECKBOX', value: 'Masspay-DEV,Masspay-SIT,Masspay-QA,Masspay-PROD', visibleItemCount: 4)    
      }
    stages {	
	    
	    stage('echo') {
		    steps {	    
		             echo "Hello World"
			     echo "${params.'Masspay-Test-Suite'}" 
		    }    
	    }
	    
               stage('build') {
            steps {
                cleanWs()
        
              script {
        def filename = "ad-123_file1.txt"   //filename will have the name of the file
        def JiraId = filename.split("_")     // JiraId will store the value that you could use at various stages 
		println(filename)   
	    String a = "Hello-World";
              String[] str;
         str = a.split('-');
      
         for( String values : str )
         println(values)	      
		      
        }  
	    }           
        }
		
		}
		
		}
