
pipeline {
agent any 
  stages {
    stage( 'abc' ){
      steps {
        sh "kubectl apply -f deploy.yml --kubeconfig /admin.conf"
      }
    }
  }
  post{
    success{
      echo "all good"
    }
    failure{
      echo "failed"
    }
    always{
      echo "always"
    }
  }
}
      
