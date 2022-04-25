
pipeline {
    agent any

    stages {
        stage('Read-JSON') {
    steps {
        script {
           
            def props = readJSON file: "${env.WORKSPACE}//file.json"
            
            //echo "$props.approver"
             String var= JSON.Parse(props);
            echo "$var[0]"
           

        }
    }
    }
}
}



