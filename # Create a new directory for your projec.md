# Create a new directory for your project (replace 'my-new-repo' with your desired repo name)
mkdir my-new-repo

# Move into the project directory
cd my-new-repo

# Initialize a new Git repository
git init

# Create a new file, for example, README.md
touch README.md

# Add the README.md file to the staging area
git add README.md

# Commit the changes
git commit -m "Initial commit"

# Set up a new repository on GitHub (replace 'username' with your GitHub username)
# You can do this manually on the GitHub website or use the following API request
# Note: You need to replace 'your_token' with your GitHub personal access token
curl -u "username:your_token" https://api.github.com/user/repos -d '{"name":"my-new-repo"}'

# Add a remote named 'origin' pointing to your GitHub repository using HTTPS
git remote add origin https://github.com/username/my-new-repo.git

# Verify that the remote has been added successfully
git remote -v

# Push the changes to the 'main' branch on GitHub (change 'main' to 'master' if needed)
git push -u origin main
