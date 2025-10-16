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
                bat 'date /T' // run shell-comand to get data
            }
        }
        stage('Stage 3: List files in workspace') {
            steps {
               bat 'dir' // run shell-command to get files list
            }
        }
        stage('Stage 4: Imitation of an error') {
            steps {
                bat 'abrakadabra' // run shell-comand to get data
            }
        }
    }
}