pipeline{
    agent any
    options{
        skipStagesAfterUnstable()
    }
    
    stages{
        stage('Build'){
            steps{
                echo 'build stage'
            }
        }
        stage('Test'){
            steps{
                echo 'test stage'
            }
        }
        stage('Deploy'){
            steps{
                echo 'deploy stage'
            }
        }
	stage('Finishing'){
	    steps{
		echo 'pipeline created successfully'
	    }
	}
    }
}
