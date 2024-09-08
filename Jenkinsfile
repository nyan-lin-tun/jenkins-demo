pipeline 
{
	agent any
	tools
	{
		maven 'MAVEN_HOME'
	}
	
	stages{
		stage('Welcome Stage')
		{
			steps
			{
				echo 'Welcome to Jenkins Pipeline'
			}			
		}
		stage('Clean Stage')
		{
			steps
			{
				sh 'mvn clean'
			}			
		}
		stage('Test Stage')
		{
			steps
			{
				sh 'mvn test'
			}			
		}
		stage('Pre-build Stage')
		{
			steps
			{
				echo 'This is pre-build stage.'
			}			
		}
		stage('Build Stage')
		{
			steps
			{
				sh 'mvn install'
			}			
		}
		stage('Post-build Stage')
		{
			steps
			{
				echo 'This is post-build stage.'
			}			
		}
		stage('Java Version Check Stage')
		{
			steps
			{
				sh 'java --version'
			}			
		}
		
		stage('Success Stage')
		{
			steps
			{
				echo 'Successfully Build Thanks'
			}			
		}
	
	}
}
