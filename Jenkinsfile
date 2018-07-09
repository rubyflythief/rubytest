#!/usr/bin/env groovy

import org.jenkinsci.plugins.pipeline.utility.steps.fs.FileWrapper
import com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition
import java.net.URLEncoder
import java.util.regex.Matcher
import groovy.transform.Field
import javax.ws.rs.core.UriBuilder

try {
node('Ruby_Linux_Node')
{
    timestamps 
    {
         stage('Run')
         {
        // Run the program
            echo "test"
        }  
    }
    finally 
    {  
        libraryClasses.NotificationUtils.notify(
        currentBuild.result)
    }
}
}

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
