pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
       stages {
           stage('build') {
               steps {
                   echo './gradlew assemble'
               }
           }
           stage('test') {
               steps {
                  echo './gradlew test'
               }
           }
       }
}
