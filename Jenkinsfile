pipeline {
    agent { label 'master' }
    
     parameters {
     
  properties([parameters([extendedChoice(description: 'Team ', multiSelectDelimiter: ',', name: 'WUBS', quoteValue: false, saveJSONParameterToFile: false, type: 'PT_CHECKBOX', visibleItemCount: 5)])])
  }
    stages {
                stage('build') {
            steps {
                echo "We can bakk: ${params.bakk}"
                echo "${bakk}"
                script {
                    if (bakk =='true') {
                echo 'I only execute on the master branch'
                } else {
                echo 'I execute elsewhere'
                    }
                
                
        }
                
                
        }
    }
}
}
