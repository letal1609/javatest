pipeline {
	agent any

    tools {
        maven 'maven_3.6.2'
    }



  stages {

    stage('Build') {
      steps {

        checkout scm

        bat '''
        mvn clean install package -X
        '''
      }
    }

  }


}
