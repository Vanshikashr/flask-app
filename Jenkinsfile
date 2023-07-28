@Library('git-shared-lib') _
kubeDeployPipeline([
  test: [
    containerRegistoryUrl: '919678485989.dkr.ecr.ap-south-1.amazonaws.com',
    yamlFilePath: 'manifest/deployment.yaml',
    gitSecret: 'token',
    gitsecret1: 'repo-clone-1',
    gitRepoUrl: 'git@github.com:AkshatTTN/flask-app.git',
    gitBranch: 'kube'
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
        fromAddress: 'sanchi.sharma1@tothenew.com',
        toAddress: 'akshat.mittal@tothenew.com'
      ]
    ]
  ]
])
// kubeDeployArgoPipeline()
