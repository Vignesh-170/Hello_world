pipeline {
    agent any
    triggers {
      scm {
        # Configuration options for triggering on push events
        includes("*") // This triggers on any branch push
      }
    }
    stages {
        stage('Run Hello World Script') {
            steps {
                script {
                    // Assuming Hello_world.py is located in the workspace
                    def output = sh(returnStdout: true, script: 'python3 Hello_world.py')
                    echo "Script output: ${output}"
                }
            }
        }
    }
}