properties([pipelineTriggers([githubPush()])])

node('linux') {     
		git credentialsId: 'github', url: 'https://github.com/infrastructure-pipeline.git', branch: 'master'
		stage('Test') { 
    sh "env"
	}   
}
