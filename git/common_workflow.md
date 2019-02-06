# A Common Git Workflow

Here's a common git workflow. If you're not doing rails, skip the
bundle/rspec pieces but run your own tests.

```bash
> git checkout master
> git pull origin master

# Make sure things still work
> bundle exec rspec spec/

# Create a new branch
> git checkout -b my_cool_new_feature

# do a work on feature here
.
> git add .
> git commit # Put in a decent commit message here please
> git push origin my_cool_new_feature

# Repeat work/add/commit/push loop until the feature is complete

# Request a PR on github
# Update code based on PR

> git push origin my_cool_new_feature

# Get approval (if you're working by yourself, you'll have to self approve

# Rebase and squash commits (Some people don't do this section of
# squashing to a single commit.
> git rebase -i master
# Squash all commits in here when vim opens
> git push -f origin my_cool_new_feature # you will need the force option here

# Merge and delete branch in *github*
> git checkout master
> git pull origin master
> bundle exec rspec spec/ # just in case
> git branch -D my_cool_new_feature

# Start on next feature!
```
