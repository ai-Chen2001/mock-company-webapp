pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
       stages {
           stage('build') {
               steps {
                   sh './gradlew assemble'
                   echo 'building application'
               }
           }
           stage('test') {
               steps {
                  sh './gradlew test'
                  echo 'test application'
               }
           }
       }
}
