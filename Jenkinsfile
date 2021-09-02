node('nodes')
}

def mavenHome = tool name: "maven 3.6.3"  
 stage('CheckoutCode')
 {
  git branch: 'development', credentialsId: 'af6db5c8-af4c-4cef-b11c-762f5060aec1', url: 'https://github.com/mss-ec-projects-aug/maven-web-application.git'
  }

 stage('Build')
 {
  sh "${mavenHome}/bin/mvn clean package"
 }
 /*
 stage('ExecuteSonarQubeReport')
 {
 sh "${mavenHome}/bin/mvn sonar:sonar"
 }
 
 stage('UploadArtifactIntoNexus')
 {
 sh "${mavenHome}/bin/mvn deploy"
 }
 
 stage('DeployAppintoTomcatServer')
 {
 sshagent(['445500f6-d277-40de-bb5d-f5f17ec05f44']) {
    sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@3.7.46.130:/opt/apache-tomcat-9.0.52/webapps/"
 }
}
}

 stage('SendEmailNotification')
 {
     
 mail bcc: 'abrarsyedp@gmail.com', body: '''Build Over

Regards,
Mithun Technologies,
7207679798''', cc: 'abrarsyedp@gmail.com', from: '', replyTo: '', subject: 'Build Over', to: 'abrarsyedp@gmail.com'
 }
*/
 
}
 
 
