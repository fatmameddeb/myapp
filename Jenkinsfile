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
