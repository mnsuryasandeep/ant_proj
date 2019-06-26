pipeline{
agent any
stages{
stage('Example') {
            steps {
                def antVersion = 'Ant'
withEnv( ["ANT_HOME=${tool antVersion}"] ) {
    sh '$ANT_HOME/bin/ant target1 target2'
}
            }
}
}
}
