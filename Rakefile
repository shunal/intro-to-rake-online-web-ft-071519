desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
  puts Student.all
  
end

task :environment do 
  require_relative './config/environment'
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
end
