node{
    stage('checkout'){
        git([url: 'https://github.com/GallonFan/maven.git', branch: 'dev'])
    }
    stage('mvn test'){
        //mvn 测试
        sh "mvn test"
    }
    stage('mvn build'){
        //mvn构建
        sh "mvn clean install -Dmaven.test.skip=true"
    }
    stage('deploy'){
        //执行部署脚本
        echo "deploy ......" 
    }
}
