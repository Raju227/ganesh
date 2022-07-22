pipeline {
    agent any
       checkout([
       $class: 'GitSCM',
       branches: scm.branches,
       doGenerateSubmoduleConfigurations: scm.doGenerateSubmoduleConfigurations,
       extensions: [[$class: 'CloneOption', noTags: false, shallow: false, depth: 0, reference: '']],
       userRemoteConfigs: scm.userRemoteConfigs,
       ])
     stages {
        stage (sample) {
           sh '''
           pwd
           ls -ltr
           '''
        }
     }
}
