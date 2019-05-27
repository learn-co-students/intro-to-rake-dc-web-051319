namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

desc 'adds environment to Rakefile'
task :environment do
  require_relative './config/environment'
end

desc 'seed database with dummy data from a seed file'
  task :seed do 
  require_relative './db/seeds'
  require_relative './lib/student.rb'
  
end 
end

namespace :greeting do 
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end
desc "outputs hola from rake to the terminal"
task :hola do 
  puts "hola de Rake!"
end
end

desc 'add a console to Rakefile'
task :console do
  puts "console"
end 
