pipeline {
    agent any

    triggers {
        // Poll SCM for changes every minute
        pollSCM('* * * * *')
    }

    stages {
        stage('Print Test Message') {
            steps {
                script {
                    // echo "hello from ${env.BUILD_USER}"
                    echo "hello from $GITHUB_ACTOR!"
                }
            }
        }
    }
}
