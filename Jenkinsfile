pipeline {
    agent all
    stages {
        stage('Source') { // Get code
            steps {
                // get code from our git repository
                git 'git@diyvb2:/home/git/repositories/workshop.git'
            }
        }
        stage('Compile') { // Compile and do unit testing
            steps {
                // run gradle to execute compile and unit testing
                sh "gradle clean compileJava test"
            }
        }
    }
}