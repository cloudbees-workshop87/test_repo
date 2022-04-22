
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
            def oldJson = '''
    { "appname": app1,
      "approver": ["gdh","gow"]
    }'''
            def props = readJSON text: oldJson
            //def keyList = props['branch'].keySet()
            echo "$props.simple"
            // println(props['branch'].keySet())

        }
    }
    }
}
}



