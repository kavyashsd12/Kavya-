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

                sh "git clone https://github.com/kavyashsd12/Kavya-.git"

            }

         }

         stage("Build"){

            steps {

                dir("Kavya-") {

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
