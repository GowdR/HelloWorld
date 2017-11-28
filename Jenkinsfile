pipeline {
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
                sh "cd /scratch/rgowd/amplify/jenkin/nodeagent"
                sh "java Hello"
            }
        }
      }
}
