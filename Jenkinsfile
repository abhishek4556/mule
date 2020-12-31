pipeline {
agent any
stages {
stage('Deploy CloudHub') {
steps {
echo 'Deploying mule project due to the latest code commit…'
echo 'Deploying to the configured environment….'
bat 'mvn package deploy -DmuleDeploy'
}
}
}
}