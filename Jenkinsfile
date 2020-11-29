node
{
  stage('scm')
   {
     git 'https://github.com/wakaleo/game-of-life.git'
    }
  stage('packaging')
  {
     sh 'mvn package'
   }
}
 stage('download test results')
  {
     junit '/target/surefire-reports/*.xml'
  }
}

