pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
          sh 'g++ ./main/helo.cpp -o ./main/hel'
          echo 'Build successful'
          build job: 'PES1UG20CS515-1'
            }
          }
stage('Test') {
    steps {
		sh './main/hello'
		echo 'Test successful'
			}
}
stage ('Deploy') {
      steps {
        echo 'Deployment Successful'
      }
   }
}
post {
    failure {
echo 'Pipeline failed'
    }
  }
}
