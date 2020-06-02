pipeline {
  agent none
  stages {
    stage('Checkout SCM') {
      checkout([$class: 'GitSCM', branches: [[name: 'master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Blog-DD/DevOpsDiggers.git']]])
    }
    // ... build stages here
  }
}
