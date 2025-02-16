pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                print "checkout"
                checkout([
                    $class: 'GitSCM'
                branches: [['*/master']]
                useRemoteConigs: [ [
                    credentialsId: 'ThophopPhe',
                    url: 'https://github.com/thiphop/CSI403-FrontEnd.git'
                ]]
                ])
                print "checkoutSuc"
            }
        }
    }
}