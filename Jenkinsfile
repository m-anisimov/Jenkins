pipeline {
    agent any
    stages {
        stage('Stage 1: Greetings'){
            steps {
                echo 'Step 1: Hello from Jenkins!'
            }
        }
        stage('Stage 2: Current date and time') {
            steps {
                bat 'date /T'
                bat 'time /T'
            }
        }
        stage('Stage 3: List files in workspace') {
            steps {
               bat 'dir' // run shell-command to get files list
            }
        }
        stage('Stage 4: File Operations') {
            steps {
               bat '''
               echo This is a test > testfile.txt
               type testfile.txt
               del testfile.txt
               '''
            }
        }
        stage('Stage 5: Network Check') {
            steps {
               bat 'ping 127.0.0.1 -n 1'
            }
       }
       stage('Stage 6: Environment variables') {
            steps {
               bat 'set'
            }
       }
       stage('Stage 7: Computername') {
            steps {
               bat 'hostname'
            }
       }
    }
}
