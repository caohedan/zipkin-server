node{
    stage('Checkout') {
        git url: 'https://github.com/tw-cloud-native/zipkin-server.git',
            branch: 'master'
    }

    withEnv([
        'SERVICE=zipkin-server'
    ]){
        stage('Deploy') {
            sh './deploy.sh'
        }
    }
}
