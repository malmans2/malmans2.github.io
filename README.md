# malmans2.github.io

Deployment instructions:

```shell
git clone https://github.com/malmans2/academic-kickstart.git My_Website
cd My_Website
git submodule update --init --recursive
rm -r public
git rm --cached public
git submodule add -f -b master https://github.com/malmans2/malmans2.github.io.git public
git add .
git commit -m "commit"
git push -u origin master
hugo
cd public
git add .
git commit -m "Build website"
git push origin master
cd ..
```
