namespace :greeting do 
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
  
  task :hola do 
    puts "hola de Rake!"
  end 
end

task :console => :environment do 
  Pry.start 
end 

task :environment do 
  require_relative 
  './config/environment'
end 

namespace :db do 
  desc 'migrate changes to our databse'
  task :migrate => :environment do 
    Student.create_table
  end
end 
