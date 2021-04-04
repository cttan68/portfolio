# Adapted from [Sidebar CV](https://github.com/jankapunkt/latexcv)

pdflatex main.tex

echo "# portfolio" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/cttan68/portfolio.git
git push -u origin main
