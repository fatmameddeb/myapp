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

