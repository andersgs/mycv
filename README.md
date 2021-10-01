## My CV

### Acknowledgments

Using a template developed by Steven V. Miller: http://svmiller.com/blog/2016/03/svm-r-markdown-cv/

### Updating

1. Update `bibfiles`
2. Replace `\textit` with `\emph` and `\Phi` to `\\Phi` --- this is needed to
  make things work nicely with the bibfile exported from Paperpile.
  The Paperpile export changes `<i>` tags to `\textit` tags, which the 
  R bibtex package does not seem to recognise. But, it does recognise the 
  `\emph` tag. In regards to `Phi`, one of the papers has the Greek letter 
  &Phi; in the title, and Paperpile exports it with the latex `\Phi` command.
  So, it needs to be escaped in order to pass the R bibtex package, and 
  be parsed correctly when knitting.
3. Update `anders-cv.Rmd` with any new achievements
4. Knit new CV
5. `git add .`
6. `git commit -m "Updated dd Month YYYY"`
7. `git tag "ddMonYYYY"`
8. `git push`
9. `git push --tags`