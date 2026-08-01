@Library('jenkins-shared-lib') _

def configMap = [
    project: "roboshop",
    component: "catalogue"
]

pipeline {
    agent {
        node { label "AGENT-1" }
    } 
    stages {
        stage('Initialize') {
            steps {
                // SCM-specific env variables require a checkout or pipeline structure to populate
                echo "Branch from environment: ${env.GIT_BRANCH ?: env.BRANCH_NAME}"
            }
        }
    }
}