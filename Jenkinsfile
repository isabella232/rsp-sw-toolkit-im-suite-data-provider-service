rrpBuildGoCode {
    projectKey = 'data-provider-service'
    testDependencies = ['mongo']
    dockerBuildOptions = ['--squash', '--build-arg GIT_COMMIT=$GIT_COMMIT']

    ecrRegistry = "280211473891.dkr.ecr.us-west-2.amazonaws.com"

    infra = [
        stackName: 'RRP-Codepipeline-DataProviderService'
    ]

    notify = [
        slack: [ success: '#ima-build-success', failure: '#ima-build-failed' ]
    ]
}