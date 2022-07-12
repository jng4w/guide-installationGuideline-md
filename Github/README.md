![jng4w](../img/jng4w.jpg)

#Github

##Overall

<p>
This guideline is for Window
</p>

##Process initializing a project

###Create README.md file
<pre>
<code>
echo "# guide-installationGuideline-md" >> README.md
</code>
</pre>

###Initialize a repository
<pre>
<code>
git init
git add .
git commit -m "first commit"
git branch -M main
</code>
</pre>

<p>
The default local branch name is "master", changing it to "main" for synchronizing with github remote repository.
</p>

###Initialize a repository
```
git remote add origin <your github link> (e.g. https://github.com/jng4w/guide-installationGuideline-md.git)
```

If remote are added, try:

```
git remote set-url origin <your github link> (e.g. https://github.com/jng4w/guide-installationGuideline-md.git)
```
###Push to remote respository
```
git push -u origin main
```

