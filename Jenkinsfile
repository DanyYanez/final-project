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
					sh 'git pull https://github.com/DanyYanez/final-project' 
				}		
			}
		}
   				
		stage('Deployment'){
			steps{
				script{
  					sh '/usr/local/bin/ansible-playbook playbook.yaml'
				}
  			}
		}
						
		stage('Testing'){
				steps{
					script {
						sh '/usr/local/bin/sleep 10' 
						sh 'kubectl get all --all-namespaces'
					}
				}				
		}
	}
}
