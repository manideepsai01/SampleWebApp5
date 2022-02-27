pipeline{
	agent any
	stages {
		stage("Git Checkout"){
       steps { git 'https://github.com/manideepsai01/SampleWebApp5.git' }
    }
    		stage("Maven Build"){
      	steps {  def mavenHome= tool name: 'maven3.6.0', type: 'maven'
        	sh "${mavenHome}/bin/mvn clean package"}
    }
}
}
