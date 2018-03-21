node { 
    git 'https://github.com/sbuvaneshkumar/testing.git'
    def sub = ["uptime","release"]
    def workspace = pwd()
    println "current workspace : ${workspace}"
    new File(workspace+"/uptime").list().each {
        if( it.contains("Jenkinsfile")){
            def jFilepath = workspace+"/uptime/" + it;
            println jFilepath
            
            def jFile = load jFilepath
            jFile.createWorkflow()
        }
    }
}
