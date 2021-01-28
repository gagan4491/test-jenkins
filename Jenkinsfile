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
                echo "Hello World!guys"
                sh 'printenv'
                sh 'pwd'
                echo "done 1"
                
        }
    }
}
}
