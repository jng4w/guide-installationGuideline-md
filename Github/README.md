<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://avatars.githubusercontent.com/u/108851604?v=4" width="100"></a></p>

#Github initialization

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
<pre>
<code>
echo "# guide-installationGuideline-md" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/jng4w/guide-installationGuideline-md.git
git push -u origin main
</code>
</pre>

