pipeline {
   environment {
        registry = "swe645docker/swe645-group-project"
        registryCredential = 'dockerID'
        TIMESTAMP = new Date().format("yyyyMMdd_HHmmss")
    }
   agent any

   stages {
      stage('Build') {
         steps {
            script{
               sh 'rm -rf *.war'
               sh 'jar -cvf studentSurveyForm.war -C main/webapp .'
               //sh 'echo ${BUILD_TIMESTAMP}'

               docker.withRegistry('https://index.docker.io/v1/', registryCredential){
                  def customImage = docker.build("averma24/studentsurveyassignment:${env.TIMESTAMP}")
               }
            }
         }
      }

      stage('Push Image to Dockerhub') {
         steps {
            script{
               docker.withRegistry('https://index.docker.io/v1/', registryCredential){
                  sh "docker push averma24/studentsurveyassignment:${env.TIMESTAMP}"
               }
            }
         }
      }

      stage('Deploying Rancher to single pod') {
         steps {
            script{
               sh "kubectl set image deployment/student-survey container-0=averma24/studentsurveyassignment:${env.TIMESTAMP}"
            }
         }
      }

      
   }
}
