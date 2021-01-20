pipeline{
    
   
    agent none
    stages{
        stage('Checkout'){
            agent any
            steps{
                git 'https://github.com/devops-trainer/DevOpsClassCodes.git'
            }
        }
        stage('Compile'){
            agent any
            steps{
                sh 'mvn compile'
            }
        }

         stage('UnitTest'){
             agent any
            steps{
                
                sh 'mvn test'
            }
            
        }
        

         stage('Package'){
            agent any
            steps{
                sh 'mvn package'
            }
            
        }
         stage('Docker Image'){
            agent any
            steps{ 
                echo 'we are in final'
                  // sh 'cd /var/lib/jenkins/workspace/ge1_code_1_cicd_stage_one_master/'
                  // sh 'sudo cp -r /var/lib/jenkins/workspace/ge1_code_1_cicd_stage_one_master/target/addressbook.war .'
                  // sh 'sudo docker build -t appimage:$BUILD_NUMBER .'
                  // sh 'sudo  docker run -itd -P appimage:$BUILD_NUMBER'
                             

          }
    }
}
}