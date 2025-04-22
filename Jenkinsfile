pipeline {
    agent any

    stages {
        stage('Show Git Info') {
            steps {
                script {
                    // Show commit hash
                    sh 'echo "Commit: $(git rev-parse HEAD)"'

                    // Show repo name
                    sh 'echo "Repo: $(basename -s .git `git config --get remote.origin.url`)"'
                }
            }
        }
    }
}
