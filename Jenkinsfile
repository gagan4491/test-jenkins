pipeline {
    agent { label 'master' }
     parameters {
     booleanParam(name: 'CAN_DANCE',
      defaultValue: true,
      description: 'Checkbox parameter')
     booleanParam(name: 'bakk',
      defaultValue: true,
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
                
                
        }
    }
}
}
