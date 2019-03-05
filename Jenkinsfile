node 
{
   stage ('build') {
   
	   withCredentials() {
        ansiblePlaybook  inventory: 'inventory', limit: '', playbook: 'playbook.yml', sudoUser: null, extras: "--vault-password rockstar007"
        }			
   }
    
}
