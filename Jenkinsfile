pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
       stages {
           stage('build') {
               steps {
                  try {
                      sh './gradlew assemble'
                  }
                  catch (exc) {
                      echo 'build failed!'
                      throw
                  }
           }
           stage('test') {
               steps {
                  try {
                      sh './gradlew test'
                  }
                  catch (exc) {
                      echo 'test failed!'
                      throw
                  }
               }
           }
       }
}
