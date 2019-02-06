#!/usr/bin/env groovy


pipeline {
    agent any
    stages {
        stage('Pinging...') {
            steps {
                sh "#!/bin/bash \n" + "ping 192.168.99.100 -c 1"
            }
        }
        stage('login to openshift...') {
            steps {
                sh "#!/bin/bash \n" + "oc login https://192.168.99.100:8443 --insecure-skip-tls-verify=true -u developer -p developer"
            }
        }
        stage('get status...') {
            steps {
                sh "#!/bin/bash \n" + "oc status"
            }
        }
        stage('logout from openshift...') {
            steps {
                sh "#!/bin/bash \n" + "oc logout"
            }
        }
    }
}
