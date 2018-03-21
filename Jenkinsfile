node {    
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'master']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sbuvaneshkumar/testing.git']]])
   // run first script
    sh 'find . -name Jenkinsfile'
    load '`find . -name Jenkinsfile 2>/dev/null | awk -F\" '{print $(NF)}'`'
    // run second script
   // load 'master/uptime/Jenkinsfile'
}
