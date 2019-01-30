pipeline {
   agent any
   stages {
      stage ('Build App' /*, compliance-check: "build-checks" */ ) {
         steps {
            echo "building"
            sh "mvn compile"
            sh "mvn test"
            sh "mvn verify"
            sh "jx step collect --pattern=target/site/jacoco/jacoco.xml --classifier=jacoco"
         }
      }
   }
}
