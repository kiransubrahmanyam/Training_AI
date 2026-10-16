git check-ignore -v .env
git add -A
git status --short
git commit -m "Ignore local environment file"
git push -u origin main