pipeline {
  agent any
    stages {
        stage('Pull') {
             steps{
                script{
                    checkout([$class: 'GitSCM', branches: [[name: '*/master']],
                        userRemoteConfigs: [[
                            credentialsId: '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',
                            url: 'https://github.com/fatmameddeb/myapp.git']]])
                }
            }
        }
}
}

