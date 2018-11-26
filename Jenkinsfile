pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          awsCodeBuild projectName: 'test-project-jekyll',
                       credentialsId: 'test-user-jekyll',
                       credentialsType: 'jenkins',
                       region: 'us-west-1',
                       sourceControlType: 'project'

        }
      }
    }
}
