pipeline{
  agent any;
  environment{
    Name = 'Akshay'
  stages{
    stage ('build'){
      steps{
        echo 
        echo "$Name"
        sh 'sleep 5'
           }
                   }
    stage ('test'){
      parallel{
        stage ('test on chrome'){
          steps{
            echo "this is parallel to test in chrome"
            sh 'sleep 5'
          }
        }
        stage ('test on ff'){
          steps{
            echo "this is parallel to test in ff"
            sh 'sleep 5'
          }
        }
      }
    }
    stage ('deploy'){
      steps{
        echo "this is deploy stage"
        sh 'sleep 5'
      }
    }
  }
}
