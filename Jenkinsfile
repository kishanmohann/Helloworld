pipeline
 {
 agent any 
 stages{
 stage('build application'){
 steps{
 bat 'mvn clean install'
 }
 }
 stage('Deploy application to mulesoft Cloudhub'){
 steps{
 bat 'mvn package deploy -DmuleDeploy'
 }
 }
 stage('Perform regression testing'){
 steps{
 bat 'C:\\Users\\vimal\\AppData\\Roaming\\npm\\newman run C:\\newman\\Helloworld.postman_collection.json --disable-unicode'
 }
 }
 }
 }