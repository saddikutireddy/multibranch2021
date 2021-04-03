
pipeline{
  agent any
  stages{
    stage('SCM Checkout'){
      steps{
          checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: '8468bb0c-b437-4f0b-8384-a4ce7ef36f92', url: 'https://github.com/saddikutireddy/my-app']]]
      }
    }
        stage('Test'){
      steps{
      echo 'job sucess'
      }
    }
  }
}
