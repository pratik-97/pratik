pipeline {
    agent any
    parameters {
        choice(name: 'executeStages', choices: ['1', '2', '3', '4', ], description: 'Select stages to execute')
    }
    stages {
        stage('Stage 1') {
            when {
                expression { params.executeStages.contains('1') }
            }
            steps {
                 echo "it is first stage"
            }
        }
        stage('Stage 2') {
            when {
                expression { params.executeStages.contains('2') }
            }
            steps {
                echo "it is second stage"
            }
        }
       
        stage('Stage 3') {
            when {
                expression { params.executeStages.contains('3') }
            }
            steps {
                echo "it is third stage"
            }
        } 

        stage('Stage 4') {
            when {
                expression { params.executeStages.contains('4') }
            }
            steps {
                echo "it is fourth stage"
            }
        }




        
        
    }
}
