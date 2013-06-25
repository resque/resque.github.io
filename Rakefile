require 'gh_contributors'

namespace :update do
  desc 'Update list of contributors'
  task :contributors do
    GhContributors.for_repo('resque/resque').to_urls.update_files('_includes/contributors.html')
  end
end 

desc "Make a new blog post"
task :blog do
  title = ENV["TITLE"] || "new-post"
  tags = ENV["TAGS"] || "[]"
  slug = title.downcase.strip.gsub(' ', '-').gsub(/[^\w-]/, '')
  date =  Time.now.strftime('%Y-%m-%d')
  filename = File.join("_posts", "#{date}-#{slug}.md")

  puts "Creating new blog post: #{filename}"
  open(filename, 'w') do |post|
    post.puts "---"
    post.puts "layout: post"
    post.puts "title: \"#{title.gsub(/-/,' ')}\""
    post.puts 'description: ""'
    post.puts "category: "
    post.puts "tags: #{tags}"
    post.puts "---"
    post.puts ""
  end
end
