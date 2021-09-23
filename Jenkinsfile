pipeline {
agent any
stages {
stage('Build') {
steps {
bat 'rm -rf build'
bat 'mkdir build' // create a new folder
bat 'echo >> car.txt' // create an empty file
bat 'echo "chassis" >> build/car.txt' // add chassis
bat 'echo "engine" >> build/car.txt' // add engine
bat 'echo "body" >> build/car.txt' // body
}
}
stage('Test') {
steps {
bat 'find "chassis" * build/car.txt'    
bat 'find "engine" * build/car.txt'
bat 'find "body" * build/car.txt'
}
}
}
}
