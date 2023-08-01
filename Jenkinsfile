@Library('git-shared-lib') _

kubeDeployArgoPipeline([
    test: [
        containerRegistoryUrl: '919678485989.dkr.ecr.ap-south-1.amazonaws.com',
        helmRepoLink: 'https://github.com/sanchi789/deveops.git',
        valuesFilePath: 'apps/values.yaml',
        gitSecret: 'token',
        gitsecret1: 'repo-clone-1',
        helmBranchName: 'main',
        scriptToRun:  '''nodejs(nodeJSInstallationName: 'Node.js 14') {
            sh \"\"\"
            npm config ls
            npm install --silent
            ls
            pwd
            echo "start building docker image"
            \"\"\"
        }'''
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
