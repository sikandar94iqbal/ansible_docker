node 
{
   stage ('build') {
   
	   withCredentials() {
        ansiblePlaybook colorized: true, credentialsId: '', forks: 10, inventory: 'inventory', limit: '', playbook: 'playbook.yml', sudoUser: null, extras: "--vault-password rockstar007"
        }			
   }
    
}
