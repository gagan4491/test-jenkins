pipeline {
    agent { label 'master' }
    
    
    options([gitLabConnection(''), [$class: 'GitlabLogoProperty', repositoryName: ''], parameters([[$class: 'ChoiceParameter', choiceType: 'PT_CHECKBOX', description: '', filterLength: 1, filterable: false, name: 'AWS', randomName: 'choice-parameter-27110276705450000']]), [$class: 'JobLocalConfiguration', changeReasonComment: '']]) 
     parameters {
     
     booleanParam(name: 'bakk',
      defaultValue: false,
      description: 'Checkbox parameter')
  }
    stages {
                stage('build') {
            steps {
                echo "We can bakk: ${params.bakk}"
                echo "${params.name}"
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
