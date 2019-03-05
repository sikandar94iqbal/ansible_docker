node 
{
   stage ('build') {
   
	
	   
	   withCredentials([string(credentialsId: 'AnsibleVaultPassword', variable: 'Secret')]) {
		   
		    
                         ansiblePlaybook  playbook: 'playbook.yml',
		         inventory: 'inventory',
		         credentialsId: "$Secret"
		   
	   }
		        
		         
   }
    
}
