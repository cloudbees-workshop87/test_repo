
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
            def oldJson = '''
    { "simple": 123,
      "fraction": 123.66,
      "exponential": 123e12
    }'''
            def props = readJSON text: oldJson
            //def keyList = props['branch'].keySet()
            echo "$props[0]"
            // println(props['branch'].keySet())

        }
    }
    }
}
}



