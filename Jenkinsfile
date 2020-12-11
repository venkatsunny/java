pipeline{
    agent any
    stages{
        stage("ECHO THINGS"){
            steps{
                withKafkaLog(kafkaServers: 'ec2-13-58-23-69.us-east-2.compute.amazonaws.com:9092', kafkaTopic: 'buildlogs', metadata:'Other info to send..') {
                echo "${env.BUILD_NUMBER}"
                echo "${env.NODE_NAME}"
                echo "venkatsunny/java"
                echo "docker demo"
              }
            
            }
        }
        
       
        
    }
}
