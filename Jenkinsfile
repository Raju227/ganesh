pipeline {
    agent any
    stages {
        stage (checkout) {
            steps {
              checkout([
              $class: 'GitSCM',
              branches: scm.branches,
              doGenerateSubmoduleConfigurations: scm.doGenerateSubmoduleConfigurations,
              extensions: [[$class: 'CloneOption', noTags: false, shallow: false, depth: 0, reference: '']],
              userRemoteConfigs: scm.userRemoteConfigs,
              ])
            }
        }
       
             
        stage (sample) {
            steps{
              
             sh '''
             pwd
             ls -ltr
             '''
          }
       }
    }
}
