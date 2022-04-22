
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
            def oldJson = '''{
            "branch":{
                "type-0.2":{"version":"0.2","rc":"1","rel":"1","extras":"1"},
                "type-0.3":{"version":"0.3","rc":"1","rel":"1","extras":"1"}
                }
            }'''
            def props = readJSON text: oldJson
            def keyList = props['branch'].keySet()
            echo "${keyList}"
            // println(props['branch'].keySet())

        }
    }
    }
}
}



