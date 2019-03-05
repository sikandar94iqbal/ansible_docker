node 
{
   stage ('build') {
   
	 
        ansiblePlaybook  playbook: 'playbook.yml',
		         inventory: 'inventory',
		         sudoUser: 'sikander',
		         extraVars: 'ansible_sudo_pass=rockstar007'
		         
   }
    
}
