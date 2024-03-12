pipeline {
    agent any

    stages {
        stage('Run Hello World Script') {
            steps {
                script {
                    // Assuming Hello_world.py is located in the workspace
                    def output = sh(returnStdout: true, script: 'python Hello_world.py')
                    echo "Script output: ${output}"
                }
            }
        }
    }
}