pipeline {
	agent any
		
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/kishori/Documents/Devops/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/pipeline.war /home/kishori/Documents/Devops/apache-tomcat-9.0.82/webapps'
			}}	
}}
