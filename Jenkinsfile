properties([pipelineTriggers([githubPush()])])

node('linux') {     
		git url: 'https://github.com/Tanya123Git/infrastructure-pipeline.git', branch: 'master'
		stage('Test')
		{ 
               		sh "env"
		} 
		stage('GetInstances')
		{
			sh "aws ec2 describe-instances --region us-east-2"
		}
		stage('CreateInstance')
		{
			sh "aws ec2 run-instances --image-id ami-013be31976ca2c322 --count 1 --instance-type t2.micro --key-name Gautam123 --security-group-ids sg-0d6a3ad9651145651 --subnet-id subnet-0fd38923f1ae916e7 --region us-east-1"
		}
	
      }
