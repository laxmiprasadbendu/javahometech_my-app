node {
  stage ('SCM Chekcout') {
    git 'https://github.com/laxmiprasadbendu/javahometech_my-app'
  }
  stage ('Compile-Package') {
    sh 'mvn package'
  }
  stage ('deploy to tomcat'){
  sshagent(['dev-ssh']) {
    sh 'scp -o StrictHostKeyChecking=no target/*.war ubuntu@172.31.43.144:/etc/tomcat8/webapp'
}
  }
  stage('email notification'){
    mail bcc: '', body: '''Hi Laxmi, Good Morning.

Thank You.''', cc: '', from: '', replyTo: '', subject: 'jenkins-notification', to: 'laxmiprasadips@gmail.com'
  }
  
  
}
  
  
  
  
  
  
  
  
  
  
