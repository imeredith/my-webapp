pipeline {
   agent any
   stages {
      stage ('Build App' /*, compliance-check: "build-checks" */ ) {
         steps {
            echo "building"
            mvn compile
         } // withMaven automatically collects jacoco reports
         // perform compliance checks related to the "Build" stage
      }

      stage ('Deploy App') {
         steps {
            echo "deploy app..."
         }
      }
   }
}
