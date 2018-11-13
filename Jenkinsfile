properties([pipelineTriggers([githubPush()])])

node('linux') {     
		git url: 'https://github.com/Tanya123Git/infrastructure-pipeline.git', branch: 'master'
		stage('Test') { 
               sh "env"
	      }   
      }
