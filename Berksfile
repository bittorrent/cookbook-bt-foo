# cookbook "chef-client", github:"opscode-cookbooks/chef-client", tag:"2.2.0"

# And now list the default places to look for cookbooks, listed in the order in
# which they'll be searched.
# Once a cookbook is found in one location, the remaining search locations will
# be ignored
chef_api :config

# Now, tell Berkshelf to include all the cookbook dependencies listed in
# metadata.rb
# Note that, from the Chef client / server's point of view, the dependencies
# listed in metadata.rb are the only ones that are considered when running this
# cookbook.
# Those earlier lines where we specified places to get particular cookbooks? And
# the search order for any non-particular cookbooks? This is the phase where
# those come into play.
metadata

# Add one more cookbook to the Berkshelf, so that it'll be available when we run
# Vagrant:
group :solo do
  cookbook "chef-solo-search", github: "edelight/chef-solo-search"
end


