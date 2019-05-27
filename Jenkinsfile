node {
    stage ("scm")
    {
    git 'https://github.com/jencyantony/maven_demo.git'
    }
    stage ("build")
    {
    bat 'mvn package'
    }    
    stage ("deploy")
    {
        echo "copy file"
        sh 'cp -R "/c/Program Files (x86)/Jenkins/workspace/PipelinescriptfromSCM/gameoflife-web/target/gameoflife.war" "/c/Program Files/Apache Software Foundation/Tomcat 8.5/webapps"'
    }
}
