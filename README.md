## BuildingSync Jekyll Site

### Local Development
1. Clone the master branch of this repo locally.
2. Run `bundle install` to install all gem dependencies (including jekyll).
3. If you are using rbenv, make sure to run `rbenv rehash`.
4. To start a local development environment, run `jekyll serve`.  Browse to http://0.0.0.0:4000 to see the site.
5. During local development, edit the code on the master branch, then refresh the browser to see your changes.
6. Commit and push the master branch when you are done.


### Deployment
We are currently using plugins that are not supported by GitHub; therefore, we cannot deploy automatically to GitHub Pages.  To deploy, follow these steps:
1. Clone the gh-pages branch of this repo locally.  This should be in a different location than your master branch clone.
2. Create a script similar to the one below:
	  ```
	  rm -rf ~/path/to/jasper-pages 
	  cd ~/path/to/BuildingSync-website-master
	  jekyll build 
	  cd ~/path/to/BuildingSync-website-gh-pages 
	  find -not -path "./.git/*" -not -name ".git" | grep git 
	  find -not -path "./.git/*" -not -name ".git" -delete 
	  cp -r ~/path/to/jasper-pages/* . 
	  cd ~ 
  	```
3. Replace the paths to the BuildingSync-website master branch, BuildingSync-website gh-pages branch, and jasper-pages (this will be one level up from the BuildingSync-website master branch, and is the location of the compiled site).
4. Run the script.  This will build the site and copy the changed files to the gh-pages branch of the repo.
5. Commit and push the gh-pages branch.


## Copyright & License

Copyright (C) 2015 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

