node {
		stage (‘Build’) {
    
			withCredentials() {

                    ansiblePlaybook(
                            playbook: "playbook.yml",
                            inventory: "inventory",
                            credentialsId: "rockstar007"
                }
      
      
		}
	}
