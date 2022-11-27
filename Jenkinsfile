pipeline{

 agent{
    label 'ansible-Node'
    }
    
  /*environment {
   AWS_EC2_PRIVATE_KEY=credentials('ec2-privatekey') 
  }*/
  

 stages{
    
    stage('checkoutcode'){
    steps{ git credentialsId: '63dafce7-0bd3-4898-8b6e-4ba004efb42c', url: 'https://github.com/00farhan00/jenkins-with-ansible.git'
    }
    }
    
    /*stage('RunAnsiblelPlaybook'){
    steps{ 
    sh "ansible-playbook -i inventory/walmart.hosts --private-key=$AWS_EC2_PRIVATE_KEY playbooks/installTomcat.yml --ssh-common-args='-o StrictHostKeyChecking=no' "
    }
    }*/
    
}//stagesclosing

}//pipelineclosing
