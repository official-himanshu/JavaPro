
pipeline{
	agent any
	options{
		skipStagesAfterUnstable()
	}
	
	stages{
		stage('Build'){
			steps{
				sh '''javac SecondJava.java'''
			}
		}
		stage('Test'){
			steps{
				sh '''echo "starting testing"
				java SecondJava
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
