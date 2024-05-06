pipeline {
	agent { docker { image 'node:13.8'} }
	stages{
		stage('Build')
		{
			steps
			{
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
