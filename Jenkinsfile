node {
      def gradleHome = tool 'GRADLE_HOME' 
stage('checkout the code from SCM')
{ 
 echo 'checkout' 
 deleteDir()
 git 'https://github.com/Raunak1015/APITestingProjectGradle.git'
} 

stage('Execute API test scripts ') 
{ 
    echo "${gradleHome}" 
    sh "${gradleHome}/bin/gradle clean test"
} 

}
