pipeline {
    agent any

    stages {
        stage('Clone GitHub Repository') {
            steps {
                script {
                    git branch: 'master',  url: "git@github.com:Alif-meem/ITMDevOps.git"
                }
            }
        }

        stage('Update Index.html') {
            steps {
                script {
                    sh 'rm /var/www/html/index.html'
                    sh 'cp -r * /var/www/html/'
                }
            }
        }
    }
}
