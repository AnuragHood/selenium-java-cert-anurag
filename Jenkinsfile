node {
	stage ('SCM checkout'){
		git "https://gitlab.com/mbabilo/experitest"
		}
	stage ('Build'){
    	dir("selenium-java-anurag") {
	   sh "mvn clean install"
       }
       	dir("selenium-java-cert-anurag/target") {
	   sh "java -jar selenium-java-anurag-1.0.7.jar"
       }
		}
}