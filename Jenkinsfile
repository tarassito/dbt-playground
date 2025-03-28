pipeline {
    agent any  // Runs on any available agent

    stages {
        stage('Hello') {
            environment {
                DB_CREDS = credentials('db_creds')
            }
            steps {
                echo 'Hello, World!'
                echo $DB_CREDS_USR
                echo $DB_CREDS_PSW
            }
        }
    }
}
