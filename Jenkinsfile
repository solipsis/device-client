pipeline {
    agent any
    stages {
        stage('build') {
            steps {
	    	sh 'echo "Building device-client"'
		sh '''
		    BUILD_DIR=$(pwd)
		    cd ..
		    rm -rf device-protocol
		    git clone -b erc20 https://github.com/keepkey/device-protocol
		    cd device-protocol
		    git pull
		    cd $BUILD_DIR
		    rm -rf build
		    npm install gulp
		    npm install
		    npm run prepublish
            ```
            }
        }
    }
}
