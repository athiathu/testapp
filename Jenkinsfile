pipeline {
    agent { label 'master' }

parameters {
        choice(name: 'BUILD_TYPE', choices: ['dev', 'release'], description: 'Select the environment for Artifactory Push')
        choice(name: 'USER', choices: ['userdebug', 'user'], description: 'Select type of user to start the build ')

    }

    stages {
        stage('build') {
            steps {
                    script{
                
                         sh '''
                            ls -la 
                            echo "${params.USER}"

                           '''

                    }

            }
        }
    }
}
