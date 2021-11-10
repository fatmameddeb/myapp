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

