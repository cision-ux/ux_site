namespace :deploy do
  def deploy(env)
    puts "Deploying to #{env}"
    system "TARGET=#{env} USER=#{ENV['usrname']} bundle exec middleman deploy  --build-before"
  end

  task :staging do
    deploy :staging
  end

  task :production do
    deploy :production
  end
end