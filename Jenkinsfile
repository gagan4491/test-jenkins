pipeline {
    agent { label 'master' }
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
