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
	def mp ="${params.'Masspay-Test-Suite'}"
	println(mp)	      
	def birdArr = [def s ="${params.'Masspay-Test-Suite'}"] as String[] 	      
	//def birdArr = ["Parrot", "Cockatiel", "Pigeon"] as String[] 
        println (birdArr[1]) // [Parrot, Cockatiel, Pigeon]	      
		      
		      
        }  
	    }           
        }
		
		}
		
		}
