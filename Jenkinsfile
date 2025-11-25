pipeline{
  agent {label 'kube-master'}
    stage{
      stage('SCM'){
        steps{
              git branch:'main',url:'https://github.com/Amith373/K8s-Jenkins_demo.git'
        }
     }
     stage('Deploy Service'){
        steps{
             sh 'kubectl apply -f '
         }
     }
     stage('Deploy pods'){
         steps{
              sh 'kubectl apply -f '
           }
        }
    }
}
