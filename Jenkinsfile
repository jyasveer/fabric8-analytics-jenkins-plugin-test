#!groovy

node {
    git url: 'https://github.com/vert-x3/vertx-mail-client.git', branch: '3.3.1'

    sh 'mvn io.github.stackinfo:stackinfo-maven-plugin:0.2:prepare'
    def response = bayesianAnalysis url: 'https://recommender.api.openshift.io/api/v1/'
    echo "Results here: ${response.getAnalysisUrl}"
}
