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
			 	docker { image "python:3.4-alpine3.8" }
			}
			steps {
				sh 'python --version'
			}
		}
	}
}
