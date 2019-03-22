#!/usr/bin/env groovy
pipeline {
	agent none
	stages {
		stage('inital') {
			steps {
				echo "只是测试项目"
			}
		}
		stage('build') {
			agent{
			 	docker { image "python" }
			}
			steps {
				sh 'python --version'
			}
		}
	}
}
