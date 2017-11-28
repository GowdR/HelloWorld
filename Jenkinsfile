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
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
