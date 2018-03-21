node {    
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'master']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sbuvaneshkumar/testing.git']]])
    // run first script
    load 'master/release/Jenkinsfile'
    // run second script
    load 'master/uptime/Jenkinsfile'
}
