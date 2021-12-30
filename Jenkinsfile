  properties([[$class: 'JobLocalConfiguration', changeReasonComment: ''], pipelineTriggers([pollSCM('*/30 * * * * ')])])
node {
    stage("clone"){
        checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/yifla/MySoftware.git']]])
    }
    stage("shoe files"){
        sh "ls -l"
    }
}
