require "rake/testtask"
require 'pathname'
require 'find'


desc 'Say hello'
task :hello do
  puts "Hello there. This is the 'hello' task."
end

desc 'Run tests'
task :default => :test

Rake::TestTask.new(:test) do |t|
  t.libs << "test"
  t.libs << "lib"
  t.test_files = FileList['test/**/*_test.rb']
end

desc 'Find not hidden files'
task :find_file do
  path_to_search = '.'
  Find.find(path_to_search) do |file|
    next if file.to_s.match(/\/\./) # next if name.include?('/.')
    puts file if File.file?(file)  # only print if is file (not dir)
  end
end



=begin

You want the Find module. Find.find takes a string containing a
path, and will pass the parent path along with the path of each file
and sub-directory to an accompanying block. Some example code:

require 'find'

pdf_file_paths = []
Find.find('path/to/search') do |path|
  pdf_file_paths << path if path =~ /.*\.pdf$/
end

That will recursively search a path, and store all file names
ending in .pdf in an array.

=end