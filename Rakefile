JAVA = "java"
JAVAC = "javac"
GROOVYC = "groovyc"
GROOVY = "groovy"
MAIN = "src/P5Script"

task :build do
  sh "#{GROOVYC} #{MAIN}.groovy"
end

task :run do
  sh "#{GROOVY} #{MAIN}.groovy"
end

task :clean do
  sh "rm -rf ./*.class ./*.swp ./*.lock"
end
