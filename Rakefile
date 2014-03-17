require 'yaml'

task :bimble do
  YAML.load_file('repos.yml').each do |repo|
    puts repo
    puts `bimble git@github.com:#{repo}.git`
  end
end

task :default => :bimble