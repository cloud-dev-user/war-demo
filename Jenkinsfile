pipeline{
	agent  { node {
                label 'node_1.4'
	}}
	stages {
	   stage("build & create package"){
               steps {
	 	 sh "mvn package"
	       	 }
		}		
           stage("tomcat deployment"){
                steps {
                   sh "cp target/devops.war /home/coder/apache-tomcat-9.0.64/webapps"				
		      }			   }		
		}
}
