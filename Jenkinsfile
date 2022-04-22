import groovy.json.JsonSlurper
Object result2;
String allDataType;
def jsonSlurper;
pipeline {
    agent any

    stages {
        stage('readjson') {
            steps {
                echo 'sending helloWorld'
                jsonSlurper = new JsonSlurper()
allDataType = '''
{ "simple": 123,
"fraction": 123.66,
"exponential": 123e12,
"null":null,
"boolean":true
}'''

result2 = jsonSlurper.parseText(allDataType)
println (result2.keySet())
                
            }
        }
    }
}



