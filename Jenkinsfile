#!/usr/bin/env groovy
pipeline {
	agent none
	stages {
		stage('inital') {
			echo "只是测试项目"
		}
		stage('build') {
			agent{
				docker { image "python:latest" }
			}
			steps {
				sh 'python --version'
			}
		}
	}
}
