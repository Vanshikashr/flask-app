// @Library('git-shared-lib') _
// DockerEcsDeploy()
@Library('git-shared-lib') _

pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                DockerEcsDeploy()
            }
        }
    }

    post {
        always {
                emailNotification()
        }
    }
}
