pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-west-2', credentials:'aws-static') {
                    // do something
                    s3Upload(bucket:"jenkinsawsudacity", includePathPattern:'*');
                }
            }
        }
    }
}
