pipeline {
    agent { label 'master' }
    stages {
        stage('Build') {
            steps {
                // Clean before build
                cleanWs()
                // We need to explicitly checkout from SCM here
                checkout scm
                echo "Building ${env.JOB_NAME}..."
            }
        }

        stage('build') {
            steps {
                echo "Hello World!"
                sh 'printenv'
                sh 'pwd'
                echo "test3ef3     done"
                
        }
    }
}
}
