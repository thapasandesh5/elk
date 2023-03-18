pipeline{
    agent any
    tools {
  terraform 'terraform'
}
stages{
    stage('Hey Git let me check you out'){
        steps{
            git branch: 'main', url: 'https://github.com/thapasandesh5/elk.git'
        }
    }
        stage('Pleasee Worrkkk'){
        steps{
            sh 'terraform init'
        }
    }
            stage('You better work'){
        steps{
            sh 'terraform apply --auto-approve'
        }
    }
}
}
