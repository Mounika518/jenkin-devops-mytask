pipeline {
	agent any
	environment{
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH ='$dockerHome/bin:$mavenHome/bin:$PATH'
 	}
	stages{
		stage('Build')
		{
			steps
			{
		      sh 'mvn --version'
			  sh 'docker version'		
              echo "Build"
			}
		}
		stage('Test')
		{
			steps
			{
              echo "Test"
			}
		}
		stage('Integration Test')
		{
			steps
			{
              echo "Integration Test"
			}
		}
	}
	
	post{
		always{
			echo 'I am awesome,I run always'
		}
        success{
			echo 'I will run when you are success'
		}
		failure{
			echo 'I will run when you fail'
		}
  	}

}	
