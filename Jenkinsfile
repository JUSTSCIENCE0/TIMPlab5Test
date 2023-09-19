pipeline {
agent any

    stages {

      stage('Cloning Git') {

        steps
          {

	   checkout scm
	  }
      }
      stage('SAST'){
	steps{
	  sh 'echo SAST stage'
	}
      }


      stage('Build-and-Tag'){


	steps{
	  sh 'echo Build and Tag'
	}
      }

      stage('Post-to-dockerhub') {
	steps {
	  sh 'echo post to dockerhub repo'
	}
      }

      stage('SECURITY-IMAGE-SCANNER'){
	steps {
	  sh 'echo scan image for security'
	}
      }

      stage('Pull-image-server') {
	steps {
	  sh 'echo pulling image ...'
	}
      }

      stage('DAST') {
	steps {
	  sh 'echo dast scan for security'
	}
      }
    }
}
