require 'yaml'

def bimble
  puts `gem install bimble`
  YAML.load_file('repos.yml').each do |repo|
    puts repo
    puts `bimble git@github.com:#{repo}.git`
  end
end

task :bimble do
  bimble
end

task :weekly do
  if Time.now.wednesday?
    bimble
  end
end

task :default do
  true
end
