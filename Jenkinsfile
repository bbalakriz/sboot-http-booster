node("launchpad-maven") {
  checkout scm
  stage("Test") {
    sh "mvn test"
  }
  stage("Deploy") {
    sh "mvn fabric8:deploy -Popenshift -DskipTests"
    # added more comments
  }
  #modified pipeline to include openshift deployment
}
