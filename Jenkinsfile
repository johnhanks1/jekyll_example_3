pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          awsCodeBuild projectName: 'builder-session-1',
                       credentialsId: 'test-user-jekyll',
                       credentialsType: 'jenkins',
                       region: 'us-west-1',
                       sourceControlType: 'project'

        }
      }
    }
}
