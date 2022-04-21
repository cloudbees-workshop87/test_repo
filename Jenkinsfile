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
    stage("Example")  {
        echo 'Hello World'
        publishEvent event: jsonEvent('{"event":"helloWorld"}')
    }
}
