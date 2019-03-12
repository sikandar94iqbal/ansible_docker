pipeline {
agent any
parameters {
      //   string(name: 'HOST', defaultValue: '/etc/fraudlens-ansible/staging', description: 'Hosts Parameters for production server')
      //   string(name: 'PASS', defaultValue: '/etc/fraudlens-ansible/group_vars/pass.yml', description: 'Passwords for production server')
      //   string(name: 'config', defaultValue: '"/etc/fraudlens-ansible/group_vars/config.yml"', description: 'Config file for Deployment')
        string(name: 'secrets', defaultValue: '"/etc/fraudlens-ansible/group_vars/secrets.yml"', description: 'secrets file for Deployment')
}
 stages{
    stage('Database-Setup') {
      steps {
        //echo "Inventory file is going to upload: $HOST"
      //   sh 'cd;'
      //   sh 'cd /etc/fraudlens-ansible/;'
        sh 'ansible-playbook playbook.yml -i inventory --tags task_1 --verbose;'
       // slackSend baseUrl: 'https://networking-zigroninc.slack.com/services/hooks/jenkins-ci/', channel: 'dl-deployment-alerts', color: 'Green', message: 'Database Build Successfully', token: 'CiNUGrFdmnNqGSNFz80YJjL3'

      }
    }

//     stage('Webserver') {
//       steps {
//         sh 'cd;'
//         sh 'cd /etc/fraudlens-ansible/;'
//         sh 'ansible-playbook -i $HOST fl_web.yml --vault-password-file=$PASS --extra-vars "config=$config secrets=$secrets" --verbose;'
//         slackSend baseUrl: 'https://networking-zigroninc.slack.com/services/hooks/jenkins-ci/', channel: 'dl-deployment-alerts', color: 'Green', message: 'Webserver Build Successfully', token: 'CiNUGrFdmnNqGSNFz80YJjL3'
//       }
//     }
//     stage('ELK') {
//       steps {
//         sh 'cd;'
//         sh 'cd /etc/fraudlens-ansible/;'
//         //sh 'ansible-playbook -i $HOST fl_elk.yml --extra-vars "config=$config"  --verbose;'
//         slackSend baseUrl: 'https://networking-zigroninc.slack.com/services/hooks/jenkins-ci/', channel: 'dl-deployment-alerts', color: 'Green', message: 'ELK Build Successfully', token: 'CiNUGrFdmnNqGSNFz80YJjL3'
//       }
//     }
//     stage('PRMS') {
//       steps {
//         sh 'cd;'
//         sh 'cd /etc/fraudlens-ansible/;'
//         //sh 'ansible-playbook -i $HOST fl_prms.yml --extra-vars "config=$config" --verbose;'

 }
}
