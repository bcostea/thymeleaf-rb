require "rake/testtask"

desc 'Run Thymeleaf benchmarks!'
task :bench do
  ruby('benchmarks/run-benchmarks.rb')
end

Rake::TestTask.new(:test) do |t|
  t.libs << "test"
  t.libs << "lib"
  t.test_files = FileList['test/**/*_test.rb']
end

task :default => :test
