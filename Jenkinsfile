def callAnt(String Parameters) {
    if (isUnix()) {
        env.PATH = "${tool 'ant'}/bin;${env.PATH}"
        sh "ant ${Parameters}"
    }
    else {
        env.PATH = "${tool 'ant'}\\bin;${env.PATH}"
        bat "ant ${Parameters}"
    }
}
pipeline{
agent any

stages{
stage('Example') {
            steps {
                        callAnt("-v -p")
            }
}
}
}
