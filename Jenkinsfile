node 
{
   stage ('build') {
   
	   withCredentials([file(credentialsId: 'vault_token', variable: 'VAULT_TOKEN')]) {
        ansiblePlaybook colorized: true, credentialsId: '', forks: 10, inventory: 'inventory', limit: '', playbook: 'playbook.yml', sudoUser: null, extras: "--vault-password rockstar007"
        }			
   }
    
}
