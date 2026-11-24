pipeline {
    agent any

    stages {
        stage('Pull Develop Code') {
            steps {
                // Pulls the Git content into 'my-target-folder' inside Jenkins workspace
                dir('my-target-folder') {
                    git branch: 'develop',
                        url: 'https://github.com/MdAkbar123/Git-Workflow-architecture',
                        credentialsId: 'github-creds' // Omit this line if your repo is public
                }
            }
        }
    }
}
