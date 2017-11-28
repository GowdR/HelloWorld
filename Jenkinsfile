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
                java Hello.java
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo 'Executing ...'
                java Hello
            }
        }
      }
}
