require 'yaml'

task :bimble do
  puts `gem install bimble`
  YAML.load_file('repos.yml').each do |repo|
    puts repo
    puts `bimble git@github.com:#{repo}.git`
  end
end

task :default do
  true
end
