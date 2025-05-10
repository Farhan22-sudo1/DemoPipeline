pipeline { 
  agent {label 'agentlinux'}
         stages {
           stages ('check version') {
             steps {
               sh "node --version"
               sh "npm --version"
             }
           }
         }
}
