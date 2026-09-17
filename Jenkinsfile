pipeline {
 agent any
 parameters {
 choice(
 name: 'ENVIRONMENT',
 choices: ['dev', 'staging', 'prod'],
 description: 'Select the deployment environment'
 )
 }
 stages {
 stage('Checkout') {
 steps {
 git branch: 'main',
 url: 'https://github.com/vaishnavik2024a-hash/ass7_p1.git'
 }
 }
 stage('Show Parameter') {
 steps {
 echo "Selected environment: ${params.ENVIRONMENT}"
 }
 }
 stage('Build for Environment') {
 steps {
 echo "Building Online Examination System for ${params.ENVIRONMENT} environment..."
 echo "Build successful."
 }
 }
 }
}
