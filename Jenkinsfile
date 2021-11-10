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


stage('Build') {
             steps{
                script{
                    sh " ansible-playbook ansible/build.yml -i ansible/inventory/host.yml"
                }
            }}
}
}
