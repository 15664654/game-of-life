pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(url: 'git@github.com:15664654/game-of-life.git', branch: 'master', changelog: true, poll: true)
      }
    }
    stage('test') {
      steps {
        echo 'test ok'
      }
    }
    stage('finish') {
      steps {
        mail(subject: 'jenkins', body: 'test pipe', from: 'chenxy@mingyuanyun.com', to: '15664654@qq.com')
      }
    }
  }
}