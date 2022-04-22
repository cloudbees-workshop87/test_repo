
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
            def oldJson = '''{
            "branch":{
                "name":{"app1"},
                "approver":{"ganga"}
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



