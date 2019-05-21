pipeline {
agent any
stages {
stages('Build') {
steps {
dir ('build') {
sh 'cmake ..'
sh 'cmake --build  .'
}
}
}
stage('Unit Tests') {
steps {
sh 'build/TestBowlingSimulator'
}
}
}
}