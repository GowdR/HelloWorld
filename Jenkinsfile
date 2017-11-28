node {
   agent {
    node {
        label 'myagent'
        customWorkspace '/scratch/rgowd/amplify/jenkin/nodeagent'
    }
  }
  
  stage('Compile') {
            steps {
                javac Hello.java 
                echo 'Compilation is successful!'
            }
        }
   
   stage('RunCode') {
            steps {
                java Hello
                echo 'Execution App is successful!'
            }
        }    
}
