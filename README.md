# First, navigate to the carbon trading platform code directory
cd /data/chats/eap5vd/workspace/carbon_trading_platform_code

# Initialize git repository
git init

# Add all files from the carbon trading platform project
git add .

# Commit all files
git commit -m "Add carbon trading platform code"

# Set the branch name to main
git branch -M main

# Add your GitHub repository as remote
git remote add origin https://github.com/darwin8259/TCC-ETS.git

# Push the entire codebase to GitHub
git push -u origin main

# Install dependencies if you haven't already
npm install

# Install gh-pages package for deployment
npm install --save-dev gh-pages

# Deploy to GitHub Pages
npm run deploy
