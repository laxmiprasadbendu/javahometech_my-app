node {
  stage ('SCM Chekcout') {
    git 'https://github.com/laxmiprasadbendu/javahometech_my-app'
  }
  stage ('Compile-Package') {
    sh 'mvn package'
  }
  stage('email notification'){
    mail bcc: '', body: '''Hi Laxmi, Good Morning.

Thank You.''', cc: '', from: '', replyTo: '', subject: 'jenkins-notification', to: 'laxmiprasadips@gmail.com'
  }
  
  
}
  
  
  
  
  
  
  
  
  
  
