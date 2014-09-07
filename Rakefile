require 'rubygems'
require 'rake'
require 'rake/testtask'

begin
  require 'rdoc/task'
rescue LoadError
  require 'rake/rdoctask'
end
require 'rspec/core/rake_task'

desc 'Default: run specs.'
task :default => :spec

desc 'Test the linode library.'
RSpec::Core::RakeTask.new('spec') do |t|
  t.pattern = 'spec/**/*_spec.rb'
end

desc 'Test the linode library.'
task :test => :spec
