# jeremy-homepage
This is the source code for my personal website, which is hosted at [zhang-jiaming.com](zhang-jiaming.com). It is built using [Hugo](https://gohugo.io/). Simply run `hugo server` to start a local server, and use your browser to see your website. The generated files will be in the `docs` folder.

## Installation and Configuration
First install Hugo
```bash
brew install hugo
```
Then clone this repository and navigate to the project folder
```bash
git clone https://github.com/jmz3/jeremy-homepage.git
cd jeremy-homepage
```
Then, configure the `hugo-coder` template theme as a git submodule
```bash
git submodule add https://github.com/luizdepra/hugo-coder.git themes/hugo-coder
```
Finally, you can run the local server
```bash
hugo server -D
```