node('slave1'){
    // Mark the code checkout 'stage'....
    stage('Checkout'){
    // Get some code from a GitHub repository
    git([url: 'https://github.com/rubyflythief/rubytest.git', branch: 'master'])
    // Mark the code build 'stage'....
    }  
    // Mark the code run 'stage'....
    stage('Run'){
    // Run the program
        echo "test"
    }
}
