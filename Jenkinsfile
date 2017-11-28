#!groovy
timestamps {
node('amplify.jenkins.slave.1.3.2') {
    stage("CodePull") {
          sh 'git clone ssh://git@cloudlab.us.oracle.com:2222/amplify/quote.git'
          checkout scm
    }
 }
}
