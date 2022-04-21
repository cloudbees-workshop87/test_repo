pipeline {
    agent any

    stages {
        stage('Example') {
            steps {
                echo 'sending helloWorld'
                publishEvent simpleEvent('helloWorld')
            }
        }
    }
}

// Script //
node {
    stage("Deploy")  {
        build job: 'CD_VIEW',
            parameters: [
                [$class: 'StringParameterValue', name: 'FROM_BUILD', value: "${BUILD_NUMBER}"]
        ]
    }
}
