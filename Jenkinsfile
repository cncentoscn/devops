#!groovy

@Library('jenkinslib@master') _

def build = new org.devops.build()

String buildShell = "${env.buildShell}"
String buildType = "${env.buildType}"

pipeline{
    agent { node { label "master"}}     
    
       
    stages{
        stage("build"){
            steps{
                script{
                    build.Build(buildType,buildShell)
                }
            } 
        }        
    } 
}      
