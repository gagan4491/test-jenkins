pipeline {
    agent { label 'master' }
    
    
    properties([gitLabConnection(''), [$class: 'GitlabLogoProperty', repositoryName: ''], parameters([[$class: 'ChoiceParameter', choiceType: 'PT_CHECKBOX', description: '', filterLength: 1, filterable: false, name: 'AWS', randomName: 'choice-parameter-27110276705450000']]), [$class: 'JobLocalConfiguration', changeReasonComment: '']]) 
     parameters {
     booleanParam(name: 'CAN_DANCE',
      defaultValue: false,
      description: 'Checkbox parameter')
     booleanParam(name: 'bakk',
      defaultValue: false,
      description: 'Checkbox parameter')
  }
    stages {
                stage('build') {
            steps {
                echo "Hello World!guys"
                sh 'printenv'
                sh 'pwd'
                echo "done "
                echo "We can dance: ${params.CAN_DANCE}"
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
