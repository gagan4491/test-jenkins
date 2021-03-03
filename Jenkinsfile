pipeline {
    agent { label 'master' }
    
     parameters {
     
     booleanParam(name: 'bakk',
      defaultValue: false,
      description: 'Checkbox parameter')
  }
    stages {
                stage('build') {
            steps {
                echo "We can bakk: ${params.bakk}"
                echo "{params.bakk}"
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
