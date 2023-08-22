@Library('git-shared-lib') _
kubeDeployPipeline([
ecrRepoName: 'main-app',
dockerFilePath: 'Dockerfile',
kube: [
  scriptToRun: '''
  whoami
  ls -la
  ''',
  containerRegistoryUrl: '336001321777.dkr.ecr.ap-south-1.amazonaws.com',
  yamlFilePath: 'manifest/deployment.yaml',
  gitSecret: 'token',
  gitSecret1: 'repo-clone-1',
  gitRepoUrl: 'https://github.com/Vanshikashr/flask-app.git',
  manifestBranchName: 'kube',
  notification: [
    [
      type: 'slack',
      webhookUrl: 'https://hooks.slack.com/services/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'
    ],
    [
      type: 'gchat',
      webhookUrl: 'https://chat.googleapis.com/v1/spaces/AAAAycUdkuk/messages?key=AIzaSyDdI0hCZtE6vySjMm-WEfRq3CPzqKqqsHI&token=KNgJ2QhUHmKD0MagNh09wfaSd3slF8-3iuBSNQVHsz0'
    ],
    [
      type: 'email',
      fromAddress: 'vanshika.shrivastava@tothenew.com',
      toAddress: 'aditya.sinha@tothenew.com'
    ]
  ]
]
])

