pipeline {
	agent any
	stages {

		stage('Create kubernetes cluster') {
			steps {
				withAWS(region:'us-west-2', credentials:'developer') {
					sh '''
						eksctl update cluster \
						--name k8scluster \
						--version 1.13 \
						--nodegroup-name standard-workers \
						--node-type t2.small \
						--nodes 2 \
						--nodes-min 1 \
						--nodes-max 3 \
						--node-ami auto \
						--region us-west-2 \
						--zones us-west-2a \
						--zones us-west-2b \
						--zones us-west-2c \
					'''
				}
			}
		}

		

		stage('Create config file cluster') {
			steps {
				withAWS(region:'us-west-2', credentials:'developer') {
					sh '''
						aws eks --region us-west-2 update-kubeconfig --name k8scluster
					'''
				}
			}
		}

	}
}
