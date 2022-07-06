pipeline {
    agent { label 'HOST_LINUX' }
    environment {
        JAVA_HOME = "/usr/lib/jvm/java-1.11.0-openjdk-amd64/"
    }

    options {
        buildDiscarder(logRotator(numToKeepStr: '10', artifactNumToKeepStr: '10'))
    }

    stages {
        stage('Setup') {
            steps {
                sh """#!/bin/env bash
                    echo 'Perform any possible setup tasks here.'
                """
            }
        }        
    }
}
