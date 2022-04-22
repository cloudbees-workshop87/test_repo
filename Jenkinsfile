import groovy.json.JsonSlurper
pipeline {
    agent any

    stages {
        stage('readjson') {
            steps {
                echo 'sending helloWorld'
                JsonSlurper jsonSlurper = new JsonSlurper()
String allDataType = '''
{ "simple": 123,
"fraction": 123.66,
"exponential": 123e12,
"null":null,
"boolean":true
}'''

Object result2 = jsonSlurper.parseText(allDataType )
println (result2.keySet())
                
            }
        }
    }
}



