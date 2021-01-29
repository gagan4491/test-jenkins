

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



        stage('build') {
            steps {
                echo "Hello World!guys"
                sh 'printenv'
                sh 'pwd'
                echo "done "
                echo 'Make the output directory'
                sh 'mkdir -p testdir'
                dir('testdir') {
                git branch: 'main', credentialsId: '91f5e3a6-48b2-4204-a476-96b771afaef3', url: 'https://github.com/gagan4491/test-jenkins.git'
      }
        }
    }
}
}
