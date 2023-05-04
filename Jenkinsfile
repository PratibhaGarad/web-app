pipeline {
     agent {
	    label {		
           label "node-1"
           customWorkspace "/mnt/new-project"
}
  }
       stages {
	     stage ("stage-1") {
		   steps {
		       sh "sudo systemctl start httpd"
			   sh "sudo cp -r index.html /var/www/html/index.html"
			   sh "sudo chmod -R 777 /var/www/html/index.html"
		 
          }		 
		 }
	   }
}
