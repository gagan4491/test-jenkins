pipeline {
    agent { label 'master' }
    
     //parameters {
     
     //booleanParam(name: 'bakk',
     // defaultValue: false,
      //description: 'Checkbox parameter')
    properties([parameters([booleanParam(defaultValue: false, description: 'Checkbox parameter', name: 'bakk')])])    
         
  //}
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
