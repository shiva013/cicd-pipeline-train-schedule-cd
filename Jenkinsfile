pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build by automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
