JAVA = "java"
JAVAC = "javac"
GROOVYC = "groovyc"
GROOVY = "groovy"

PACKAGE = "p5sc"
SRC = "src"
CLASSES = "classes"

MAIN = "Main"
ENTRY = "P5Script"
CLASSPATH = ".:#{CLASSES}:lib"

task :build => [:clean] do
  sh "mkdir -p #{CLASSES}"
  sh "#{GROOVYC} -cp #{CLASSPATH} #{SRC}/#{ENTRY}.groovy -d #{CLASSES}"
  sh "#{JAVAC} -cp #{CLASSPATH} #{SRC}/#{MAIN}.java -d ."
end

task :groovy do
  sh "#{GROOVY} -cp #{CLASSPATH} #{SRC}/#{MAIN}.groovy"
end

task :java do
  sh "#{JAVA} -cp #{CLASSPATH} #{MAIN}"
end

task :clean do
  sh "rm -rf ./*.class ./*.swp ./*.lock #{CLASSES}"
end
