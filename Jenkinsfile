@Library("jenkins-shared-library_raghu@main") _
pipeline {

    agent any
		stages {

			stage('Build') {
				steps {
                    dotnet("test")	
			}
		}
		
			stage ('Publish'){
				steps {
					dotnet("publish")
				}
			}
      
	}
}
