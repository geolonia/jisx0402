require 'rake/testtask'

task :default => :gen_json

desc "generate JSON file"
task :gen_json do
  ruby "build.rb"
end

Rake::TestTask.new do |t|
  t.libs << "test"
  t.test_files = FileList['test/test*.rb']
  t.verbose = true
end
