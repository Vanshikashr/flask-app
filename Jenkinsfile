@Library('git-shared-lib') _
DockerEcsDeploy([ 
  appName: 'new-app',
  dockerFilePath: 'docker/Dockerfile',
  main: [
    containerRegistoryUrl: '919678485989.dkr.ecr.ap-south-1.amazonaws.com',
    clusterName: 'jen-cluster',
    serviceName: 'demo-svc2',
    taskDefinition: 'demo-task2',
    notification: [
      [
        type: 'email',
        fromAddress: 'sanchi.sharma1@tothenew.com',
        toAddress: 'akshat.mittal@tothenew.com'
      ]
    ]
  ]
])
// DockerEcsDeploy()
