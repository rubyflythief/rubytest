#!/usr/bin/env groovy

/*import org.jenkinsci.plugins.pipeline.utility.steps.fs.FileWrapper
import com.cwctravel.hudson.plugins.extended_choice_parameter.ExtendedChoiceParameterDefinition
import java.net.URLEncoder
import java.util.regex.Matcher
import groovy.transform.Field
import javax.ws.rs.core.UriBuilder
*/
import java.io.File
node('Ruby_Linux_Node')
{
    timestamps 
    {
         stage('Build')
            {
                // Run the program
                echo "test"
             }
        stage('Run Exception')
                {
                    try{
                        echo 'Catch exception'
                        //find a non-exit file
                        File source = new File("/home/test.txt")
                    }catch (e){
                        echo 'failed due to $e'
                    }finally{
                        echo 'test done'
                    }
                }
    }

}



