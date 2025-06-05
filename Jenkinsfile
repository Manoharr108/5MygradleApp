pipeline{
	agent any
	tools{
		jdk 'jdk'
		gradle 'gradle'
	}
	stages{
		stage('Checkout'){
			steps{
				git branch: 'master' , url :'https://github.com/Manoharr108/5MygradleApp'
			}
		}
		stage('Build'){
			steps{
				sh 'gradle build'
			}
		}
		stage('Test'){
			steps{
				sh 'gradle test'
			}
		}
		stage('Run Application'){
			steps{
				sh 'gradle run'
			}
		}
	}
}
