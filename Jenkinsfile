pipeline {
agent any
stages {
stage('Test') {
steps {
echo 'Application in Testing Phase…'
bat 'mvn test'
}
}
stage('Deploy CloudHub') {
steps {
echo 'Deploying mule project due to the latest code commit…'
echo 'Deploying to the configured environment….'
bat 'mvn package deploy -DmuleDeploy'
}
}
}
}