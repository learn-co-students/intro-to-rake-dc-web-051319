# require_relative "./config/environment.rb"

desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :greeting do
  desc "Outputs hello to the terminal but with namespacing!"
  task :hello do
    puts "hello from Rake!"
  end
  
  desc "Outputs hola to the terminal"
  task :hola do
    puts "hola de Rake!"
  end
end

desc "Starts binding.pry in the terminal"
task :console do
end

namespace :db do

  desc "Invokes the environment task as dependency"
  task :migrate => :environment do
  end



  # desc 'seed the database with some dummy data'
  # task :seed do
  #   require_relative './db/seeds.rb'
  # end

  desc "Seed Invoke"
  task :seed do
    require_relative "./db/seeds.rb"
  end

  desc "dependency"
  task :environment do
    puts "In environment"
  end

end