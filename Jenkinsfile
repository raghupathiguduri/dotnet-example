@Library("jenkins-shared-library_raghu@main") _
pipeline {

    agent any
		stages {

			stage('Build') {
				steps {
                    dotnetBuild("test")	
			}
		}
		
			stage ('Publish'){
				steps {
					dotnetBuild("publish")
				}
			}
      
	}
}
