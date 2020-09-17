pipeline{
	agent any
	options{
		skipStagesAfterUnstable()
	}
	
	stages{
		stage('Build'){
			steps{
				sh '''javac SimpleJava.java'''
			}
		}
		stage('Test'){
			steps{
				sh '''echo "starting testing"
				java SimpleJava
				echo "testing finished"'''
			}
		}
		stage('Deploy'){
			steps{
				echo "all test case passes"
				echo "Starting deploy stage"
				echo "--------Processing----------"
				echo "Deploy finish"
			}
		}
	}
}
