
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
            def oldJson = '''{
            {
            "smoke": "Test1.js",
            "default": "Test2.js"
            }
            }'''
            def props = readJSON text: oldJson
            //def keyList = props['branch'].keySet()
            echo "${keySet}"
            // println(props['branch'].keySet())

        }
    }
    }
}
}



