@Library('git-shared-lib') _
kubeDeployPipeline([
ecrRepoName: 'main-app',
dockerFilePath: 'Dockerfile',
scriptToRun: '''
  whoami
  ls -la
  ''',
kube: [
  containerRegistoryUrl: '919678485989.dkr.ecr.ap-south-1.amazonaws.com',
  yamlFilePath: 'manifest/deployment.yaml',
  gitSecret: 'token',
  gitSecret1: 'repo-clone-1',
  gitRepoUrl: 'https://github.com/AkshatTTN/flask-app.git',
  manifestBranchName: 'kube',
  notification: [
    [
      type: 'slack',
      webhookUrl: 'https://hooks.slack.com/services/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'
    ],
    [
      type: 'gchat',
      webhookUrl: 'https://chat.googleapis.com/v1/spaces/AAAAycUdkuk/messages?key=AIzaSyDdI0hCZtE6vySjMm- 
                   WEfRq3CPzqKqqsHI&token=KNgJ2QhUHmKD0MagNh09wfaSd3slF8-3iuBSNQVHsz0'
    ],
    [
      type: 'email',
      fromAddress: 'sanchi.sharma1@tothenew.com',
      toAddress: 'akshat.mittal@tothenew.com'
    ]
  ]
]
])
// kubeDeployArgoPipeline()
