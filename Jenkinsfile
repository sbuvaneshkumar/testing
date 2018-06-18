pipeline {
	agent any 
	stages{
stage('Code Checkout') {
                                checkout scm
                                repositoryURL = sh(script: 'git config remote.origin.url', returnStdout: true).trim()
                                echo "${repositoryURL}"
                                repositoryName = sh (script: "echo ${repositoryURL} | rev | cut -d '.' -f2 | cut -d '/' -f1 | rev ", returnStdout: true).trim()
                                echo "${repositoryName}"
            			}

