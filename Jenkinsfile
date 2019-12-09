pipeline {
  agent any
  stages {
    stage('readfile') {
      steps {
        ws(dir: 'D:\\soft\\jenkins')
        readFile(file: '1.txt', encoding: 'utf-8')
      }
    }

    stage('deployed') {
      steps {
        emailext(attachLog: true, subject: 'jenkins', body: 'test succeed', to: '2524207241@qq.com')
      }
    }

  }
}