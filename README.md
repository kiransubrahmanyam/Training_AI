git remote set-url origin https://github.com/kiransubrahmanyam/Training_AI.git

# Add .env to .gitignore if it isn't already there
grep -qxF '.env' .gitignore || printf '%s\n' '.env' >> .gitignore

git check-ignore -v .env
git add -A
git status --short
git commit -m "Ignore local environment file"
git push -u origin maingit check-ignore -v .env