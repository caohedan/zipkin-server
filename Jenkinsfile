node{
    stage('Checkout') {
        checkout scm
    }

    withEnv([
        'SERVICE=zipkin-server'
    ]){
        stage('Deploy') {
            sh './deploy.sh'
        }
    }
}
