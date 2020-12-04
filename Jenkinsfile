pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                echo "Hello World!"
                 sh '''
            #!/bin/bash
            printenv
            
         '''
    }
            }
        }
    }
}

