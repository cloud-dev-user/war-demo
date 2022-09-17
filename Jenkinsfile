pipeline{
        agent { label "linux" }
		stages {
		   stage("build & create package"){
                steps {
				 sh "mvn package"
				 }
				 }		
           stage("tomcat deployment"){
                steps {
                   sh "cp target/devops.war /home/coder/apache-tomcat-9.0.64/webapps"				
		               }
					   }		
		}
}
