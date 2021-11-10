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

