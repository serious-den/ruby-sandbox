task :purchaseAlchohol do
  puts "00000000000"
end

task :mixDrink do
  puts "11111111"
end

task :getSmashed do
  puts "22222222222222"
end

task :default do
  puts "def !!!"
end

require 'rake/testtask'

=begin
require 'ci/reporter/rake/rspec'     # use this if you're using RSpec
require 'ci/reporter/rake/cucumber'  # use this if you're using Cucumber
require 'ci/reporter/rake/spinach'   # use this if you're using Spinach
require 'ci/reporter/rake/test_unit' # use this if you're using Test::Unit
=end
require 'ci/reporter/rake/minitest'  # use this if you're using Ruby 1.9 or minitest

Rake::TestTask.new(:test) do |t|
  t.libs << "test"
  t.test_files = FileList['tests/*.rb']
  t.verbose = true
end

=begin
task :test => ['ci:setup:testunit'] do |t|
  t.libs << "tests"
  t.test_files = FileList['tests/*.rb']
  t.verbose = true
end
=end

