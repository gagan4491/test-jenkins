pipeline {
    agent { label 'master' }
    stages {
        stage('pre build') {
            steps {
                // Clean before build
                cleanWs()
                // We need to explicitly checkout from SCM here
                checkout scm
                echo "Building ${env.JOB_NAME}..."
            }

        }

       stage('clone') {
            dir('CalibrationResults') {
            git url: 'https://github.com/gagan4491/test-jenkins.git'
    }
    }

        stage('build') {
            steps {
                echo "Hello World!guys"
                sh 'printenv'
                sh 'pwd'
                echo "done "
                
        }
    }
}
}
