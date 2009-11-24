require 'rake'
require 'fileutils'
include FileUtils

desc 'Install into home directory'
task :install do
  Dir.foreach("bin/") do |f|
    install File.join('bin/', f), '/home/silas/bin', :mode => 0755, :verbose => true if f =~ /^[^\.]/
  end
end
