pipeline {
    agent any
    options {
        buildDiscarder(logRotator(daysToKeepStr: '10', numToKeepStr: '10'))
        timeout(time: 12, unit: 'HOURS')
    }
    stages {
        stage("Welcome!") {
            steps {
                echo "You reached the GitHub Account of Henry-NS-2021."
              echo "creating a file..."
              sleep 5
                writeFile file: 'auto_generated_file.txt', text: "file generated by a job triggered on Jenkins"
            }
        }
          stage("finishing the job"){
            steps{
              sleep 3
              echo "job finishin in 3 sec"
            }
          }
    }
}
