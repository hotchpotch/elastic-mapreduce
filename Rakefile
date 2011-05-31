# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "elastic-mapreduce"
  gem.homepage = "http://github.com/hapyrus/elastic-mapreduce"
  gem.license = "Apache License"
  gem.summary = %Q{Amazon's commandline client for EMR (Elastic Map-Reduce) invocation (Unofficial Gem and Ruby 1.9 Version)}
  gem.description = %Q{Original is official but this is Unofficial gem.}
  gem.email = "fujibee@hapyrus.com"
  gem.authors = ["Amazon.com", "Koichi Fujikawa"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/test_*.rb'
  test.verbose = true
end

task :default => :test
