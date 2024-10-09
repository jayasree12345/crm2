pipeline{
  agent any
  stages{
    stage("Maven Build"){
      when{
        branch 'develop'
      }
      steps{
        echo "maven build...."
      }
    }
    stage("Sonar Analysis"){
      when{
        branch 'develop'
      }
      steps{
        echo "sonar analysis...."
      }
    }
    stage("Vulnarability Scanning"){
      when{
        branch 'develop'
      }
      steps{
        echo "vulnarability scanning...."
      }
    }
    stage("Dev Deploy"){
      when{
        branch 'develop'
      }
      steps{
        echo "dev deploy...."
      }
    }
    stage("Test Deploy"){
      when{
        branch 'test'
      }
      steps{
        echo "test deploy...."
      }
    }
    stage("Prod Deploy"){
      when{
        branch 'main'
      }
      steps{
        echo "prod deploy...."
      }
    }
  }
}
