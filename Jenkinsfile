node 
{
   stage ('build') {
   
	
	   
	   withCredentials([string(credentialsId: 'AnsibleVaultPassword', variable: 'Secret')]) {
		   
		    
                                      ansiblePlaybook vaultCredentialsId: 'abc123', inventory: 'inventory', playbook: 'playbook.yml'
		   
	   }
		        
		         
   }
    
}