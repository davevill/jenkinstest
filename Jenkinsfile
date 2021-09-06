pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(3) {
                    bat 'cp nofound nofound2'
                }

                timeout(time: 3, unit: 'MINUTES') {
                    bat 'ping google.com'
                }
            }
        }
    }
}
