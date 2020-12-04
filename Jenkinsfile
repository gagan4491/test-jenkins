pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                echo "Hello World!"
                sh "$pwd"
                }
            stage('first') {
            agent { label 'master' }
            steps {
               sh "printenv | sort"
            }
        }
    }
}
}
