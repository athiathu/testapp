pipeline {
    agent { label 'master' }

parameters {
        choice(name: 'BUILD_TYPE', choices: ['dev', 'release'], description: 'Select the environment for Artifactory Push')
        choice(name: 'USER', choices: ['userdebug', 'user'], description: 'Select type of user to start the build ')
        choice(choices: ['US-EAST-1', 'US-WEST-2'], description: 'What AWS region?', name: 'region')

    }

    stages {
        stage('build') {
            steps {
                    script{
                
                             sh "echo ${params.region}"


                    }

            }
        }
    }
}
