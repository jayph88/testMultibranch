node('master')
{
     //env.XML = ReadFile ('TEST-JSystem_JUnit_report.xml')
     //def xml = ${env.XML}
     checkout scm
     sh 'cat Jenkinsfile'
     def xml = readFile ('TEST-JSystem_JUnit_report.xml')
     def rootNode = new XmlParser().parseText(xml)
     println (rootNode.@failures)
    
}
