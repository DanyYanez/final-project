pipeline {
			agent any
			
			stages {
				stage('Clean workspace'){
					steps{
						script{
							sh 'rm -rf $PWD/case2'						
						}
					}
				}
				stage('Cloning Repo'){
					steps {
						script{
							sh 'git clone https://github.com/DanyYanez/final-project' 
						}		
					}
				}
				
	 
   				stage('Deployment'){
					steps{
  						ansiblePlaybook installation: 'Ansible', playbook: 'playbook.yaml'
  }
}

        						
			stage('Testing'){
				steps{
					script {
						sh '/usr/local/bin/kubectl get all --all-namespaces'
					}
				}				
			}
		}
	}
