pipeline {
    agent any
    parameters {
            choice(name: 'BRANCH', choices:['feature/revamp'], description: 'feature branch name')
            string(name: 'VERSION_NAME', defaultValue: '8.12.1', description: 'feature/revamp version name')
            string(name: 'VERSION_CODE', defaultValue: '2147483647', description: 'feature/revamp version code')
            choice(name: 'ENV', choices:['StagUnpinned','ProdUnpinned','StagPinned','ProdPinned'], description: 'build envrionment')
            choice(name: 'BUILD_MODE', choices:['Debug','Release'], description: 'build mode')
            choice(name: 'APK_PATH', choices:['stagUnpinned/debug','stagUnpinned/release','prodUnpinned/debug','prodUnpinned/release','stagPinned/release','prodPinned/release'], description: 'apk path')
            choice(name: 'APK_NAME', choices:['app-stag-unpinned-debug','app-stag-unpinned-release','app-stag-pinned-release','app-stag-pinned-debug','app-prod-unpinned-release','app-prod-unpinned-debug','app-prod-pinned-release','app-prod-pinned-debug'], description: 'apk name')
            string(name: 'MODULE_NAME', defaultValue: 'app')
    }
    stages {
        stage('Example') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}