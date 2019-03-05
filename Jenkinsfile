node 
{
   stage ('build') {
   
	
	   
	   withCredentials([string(credentialsId: 'AnsibleVaultPassword', variable: 'Secret')]) {
		   
		    
                                              ansiblePlaybook credentialsId: 'abc123', inventory: 'inventory', playbook: 'playbook.yml'
		   
	   }
		        
		         
   }
    
}
