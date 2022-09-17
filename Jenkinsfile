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
                   sh "cp ${env.WORKSPACE}/target/devops.war /opt/tomcat9/apache-tomcat-9.0.64/webapps/"				
		      }			   }		
		}
}
