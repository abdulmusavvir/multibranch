pipeline{
 agent any
 stages{
    stage('common'){
      steps{
      echo 'common for all'
      }
    }
    stage('build for main'){
       when{
            expression{
                BRANCH_NAME == 'main'
            }
            }
       steps{
            echo 'Build for main'
            }
    }
    stage('build for dev'){
       when{
            expression{
                BRANCH_NAME == 'dev'
            }
            }
       steps{
            echo 'Build for dev'
            }
    }
    stage('build for Feature'){
       when{
            expression{
                BRANCH_NAME == 'feature'
            }
            }
       steps{
            echo 'Build for Feature'
            }
    }
   }
  }
