#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                echo 'Hello World ...'
                sh "#!/bin/bash \n" + "ping 192.168.99.100 -c 1"
            }
        }
    }
}
