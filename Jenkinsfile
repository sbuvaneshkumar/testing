node {    
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sbuvaneshkumar/testing.git']]])
    // run first script
    load 'release/Jenkinsfile'
    // run second script
    load 'uptime/Jenkinsfile'
}
