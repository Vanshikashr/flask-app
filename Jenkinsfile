// @Library('git-shared-lib') _
// DockerEcsDeploy()
@Library('git-shared-lib') _
DockerEcsDeploy()
pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                echo "Hello happy Pipeline"
            }
        }
    }

    post {
        always {
                emailNotification()
        }
    }
}
