pipeline
{
agent any
stages
{
  stage('code scm checkout')
  { steps{ git branch: 'master', url: 'https://github.com/Satya7340/gradle-calculator'}
  }
  
  stage('code build')
  { steps{sh './gradlew clean build'
          sh './gradlew jar'
		  sh './gradlew test'}
  }

}

}
