JAVA = "java"
JAVAC = "javac"
GROOVYC = "groovyc"
GROOVY = "groovy"
MAIN = "src/P5Script"
CLASSPATH = ".:./lib"

task :build do
  sh "#{GROOVYC} -cp #{CLASSPATH} #{MAIN}.groovy"
end

task :run do
  sh "#{GROOVY} -cp #{CLASSPATH} #{MAIN}.groovy"
end

task :clean do
  sh "rm -rf ./*.class ./*.swp ./*.lock"
end
