pipeline {
	agent any 
	stages{
stage('print output') {
	steps{
		script{
  sh (script: cat /var/log/dpkg.log', returnStdout: true).trim())
}
}
}
	}}
