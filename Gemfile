source 'https://rubygems.org'

gemspec

case ENV["DB"]
when "mysql"
  gem "mysql2"
when "postgres"
  gem "pg"
else
  gem "sqlite3"
end
