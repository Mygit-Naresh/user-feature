#!groovy
@Library('roboshop-shared-library') _
def configMap = [
    application: "nodejsVM",
    component: "user"
]
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipeline(configMap)
}
else{
    echo "This is PRODUCTION, deal with CR process"
}
// nodejsVM()