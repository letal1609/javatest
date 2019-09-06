pipeline {
	agent any

    tools {
        maven 'maven_3.6.2'
    }



  stages {

    stage('Build') {
      steps {

        checkout scm

        sh '''
        mvn clean install package -X
        '''
      }
    }

  }


}
