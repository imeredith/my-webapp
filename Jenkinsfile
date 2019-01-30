pipeline {
   agent any
   stages {
      stage ('Build App' /*, compliance-check: "build-checks" */ ) {
         steps {
            echo "building"
            mvn compile
         }
      }
   }
}
