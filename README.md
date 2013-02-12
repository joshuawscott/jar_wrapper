# Jar Wrapper -- Jar wrapper for executable java jarjava jar

## Installing Jar Wrapper

    $ gem install jar_wrapper

## Usage

require 'jar_wrapper'

wrapper = JarWrapper::Runner.new
wrapper.java_opts = ["-Xmx1024m", "-Xss1024k" ]

1. install jar file from source URL into target file:

wrapper.install source, target

2. execute jar file (java -jar jar_file):

wrapper.jar_file = jar_file
wrapper.run ARGV

3. execute main class (java -cp ... main_class):

wrapper.classpath = some_class_path
wrapper.main_class = main_class
wrapper.run ARGV


      
