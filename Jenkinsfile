
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
           
            def props = readJSON file: "${env.WORKSPACE}//file.json"
            
            //echo "$props.approver"
            echo "$substringAfter("Hello World", " ")"
            //echo "$substringAfter("$props.approver", ",")"
             //String var= "$props.approver"
            
            //echo "$var[0]"
           

        }
    }
    }
}
}



