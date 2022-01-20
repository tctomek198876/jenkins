pipeline {
         agent any
         
            parameters{
                booleanParam(name: 'ELK', defaultValue: false, description: 'Checkbox parameter', )
                //choice(choices: 'sprint_6\nsprint_7\nsprint_8\nSprint_9', description: 'Select branch to Build', name: 'Branch')
                //choice(choices: 'No\nYes', , name: 'choice2')
				stringParam('myParameterName', 'my default stringParam value', 'my description')
              }
         
         stages {
                 stage('Build') {
                 steps {
                     echo 'Hi, GeekFlare. Starting to build the App.'
                 }
                 }
                 stage('Test') {
                 steps {
                    echo "Start the deploy .."
                 }
                 }
                 stage('Deploy') {
                 parallel { 
                            stage('Deploy start ') {
                           steps {
                                echo "Start the deploy .."
                           } 
                           }
                            stage('Deploying now') {
                            
                              steps {
                                echo "Docker Created"
                              }
                           }
                           }
                           }
                 stage('Prod') {
                     steps {
                                echo "App is Prod Ready"
                              }
                 
              }
}
}

