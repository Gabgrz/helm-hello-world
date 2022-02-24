#!/usr/bin/env groovy

pipeline {
    agent {
        label 'centos7-with-docker'
    }
    stages {
        stage('Setup') {
            steps {
                echo "Setup step";
                script {
                    def dockerSandbox = docker.image('dtzar/helm-kubectl:3.7.2')
                    dockerSandbox.pull()
                    dockerSandbox.inside () {
                        sh "id"
                        sh "pwd"
                        sh "ls -l"
                        sh "helm version"
                    }
                }
            }
        }
    }
}