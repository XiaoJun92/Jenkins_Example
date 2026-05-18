pipeline {
    agent any

    stages {
        stage('Check out') {
            steps {
                echo '拉取代码中...'
                // 如果在 Jenkins 任务中勾选了 "Pipeline syntax" 从 SCM 获取，这一步甚至可以省略
                git branch: 'main', url: 'git@github.com:XiaoJun92/Jenkins_Example.git'
            }
        }

        stage('Build') {
            steps {
                echo '开始编译项目...'
                // 根据你的现有项目类型执行编译：
                // 如果是 Java Maven 项目: sh 'mvn clean package'
                // 如果是 Node.js 前端项目: sh 'npm run build'
                sh 'echo "Building..."'
            }
        }
    }
}