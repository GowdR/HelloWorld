#!groovy
timestamps {
node('amplify.jenkins.slave.1.3.2') {
    agent {
    node {
        label 'myagent'
        customWorkspace '/scratch/rgowd/amplify/jenkin/nodeagent'
    }
   }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Compiling ...'
                sh "javac Hello.java"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'Executing ...'
                sh "java Hello"
            }
        }
      }
}
}
