pipeline {
    agent any
    stages{
        stage('Run Postman collection with Taurus newman executor') {
            steps{
                sh 'sudo docker run --privileged=true --rm  ' +
                        '-v $pwd/bzt-config:/bzt-configs ' +
                        'blazemeter/taurus ' +
                        'run_postman_collection.yml'
            }
        }

    }

}