node {
  stage ('SCM Chekcout') {
    git 'https://github.com/laxmiprasadbendu/javahometech_my-app'
  }
  stage ('Compile-Package') {
    sh 'mvn package'
  }
  stage('email notification'){
    mail bcc: '', body: '''Hi Laxmi Prasad
How are you ?''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'laxmiprasadips@gmail.com'
  }
  
}
  
  
  
  
  
  
  
  
  
  
