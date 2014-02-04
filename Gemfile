source 'https://rubygems.org'

gemspec

case ENV["DB"]
when "mysql"
  gem "mysql2"
when "postgres"
  platforms :mri do
    gem "pg", "0.15.1"
    gem "sequel_pg", "1.6.8"
  end
  platforms :jruby do
    gem "jdbc-postgres"
  end
else
  gem "sqlite3"
end
