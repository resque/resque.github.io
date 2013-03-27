require 'gh_contributors'

namespace :update do
  desc 'Update list of contributors'
  task :contributors do
    GhContributors.for_repo('defunkt/resque').to_urls.update_files('_includes/contributors.html')
  end
end 
