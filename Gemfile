source :rubygems

require 'rbconfig'

def windows?
  !!(RbConfig::CONFIG['host_os'] =~ /mswin|mingw|windows/)
end

gem "rubyzip"

group :development do
  gem "gemspec_deps_gen"
  gem "gemcutter"
end

group :test do
  gem "rspec"
  gem "mocha"
end



