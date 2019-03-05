node 
{
   stage ('build') {
   
	
	   
	   withCredentials([string(credentialsId: 'AnsibleVaultPassword', variable: 'Secret')]) {
		   
		    
                         ansiblePlaybook  playbook: 'playbook.yml',
		         inventory: 'inventory',
		         vaultCredentialsId: '${AnsibleVaultPassword}', 
                         extras : "--ask-vault-pass ${AnsibleVaultPassword}"
		   
	   }
		        
		         
   }
    
}
