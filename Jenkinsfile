pipeline{

    agent any

    stages {

         stage("Clean Up "){

            steps {

                deleteDir()

            }

         }

         stage("Clone Repo"){

            steps{

                sh "git clone https://github.com/kavyashsd12/Kavya-.git/simple-java-maven-app"

            }

         }

         stage("Build"){

            steps {

                dir("simple-java-maven-app") {

                    sh "mvn clean install"

                }

            }

         }

         stage("Test"){

            steps{

                dir("simple-java-maven-app") {

                    sh "mvn test"

                }

            }

         }

    }

}
