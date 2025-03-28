pipeline {
    agent any

    stages {
        stage('Run Only for PR to Develop') {
            when {
                allOf {
                    changeRequest target: 'develop'
                }
            }
            steps {
                echo "This stage runs only for PRs targeting 'develop' branch!"
            }
        }

        stage('Always Runs') {
            steps {
                echo "This stage runs for all builds."
                sh 'printenv'
            }
        }
    }
}
