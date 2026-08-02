@Library('jenkins-shared-lib') _

def configMap = [
    project: "roboshop",
    component: "catalogue"
]

if ( ! env.GIT_BRANCH.equalsIgnoreCase("main") ){
    nodejsEKSPipeline(configMap)
}
else {
    echo "need permision"
}