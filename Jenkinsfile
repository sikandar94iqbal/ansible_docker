node 
{
   stage ('build') {
   
	 
        ansiblePlaybook  playbook: 'playbook.yml',
		         inventory: 'inventory',
		         sudoUser: 'sikander',
		         extras: "ansible_sudo_pass=rockstar007"
   }
    
}
