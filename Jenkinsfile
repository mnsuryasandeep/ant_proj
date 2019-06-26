pipeline{
agent any
def antVersion = 'Ant'
stages{
stage('Example') {
            steps {
withEnv( ["ANT_HOME=${tool antVersion}"] ) {
    sh '$ANT_HOME/bin/ant target1 target2'
}
            }
}
}
}
