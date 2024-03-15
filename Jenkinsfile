pipeline {
    agent any
    stages {
        stage('Input') {
            steps {
                script {
                    curl 'https://raw.githubusercontent.com/elastic/examples/master/Common%20Data%20Formats/apache_logs/apache_logs' | grep '\<logstash.*HTTP/1\.1" 200\>' -c
                }
            }
        }
    }
}