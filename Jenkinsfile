@Library("jenkins-shared-library_raghu@main") _
pipeline {

    agent any
		stages {

			stage('Build') {
				steps {
                    Builddotnet("test")	
			}
		}
		
			stage ('Publish'){
				steps {
					Builddotnet("publish")
				}
			}
      
	}
}
