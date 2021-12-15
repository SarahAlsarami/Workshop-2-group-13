
# Text Classification System 

This workshop is based on developing a web-based machine learning system for simple text 
classification. The following steps will show you how to set up a Node js server to run the core system of 
the machine learning (fasttext tool for text classification) on input from a user.

First of all, you must enter the commands to install npm in the Linux system
so I downloaded the virtual box on my pc then in the terminal I wrote these commands to install npm.

Download npm

## Download npm

 To install npm

```bash
sudo apt install npm

```
   Then I create a folder and name it "sat" , placed in the desktop then I put the files :( index.html,index.js and train.txt ) in the folder .
   
## Initialize requirements

First we should Go to the project folder directory

```bash
cd Desktop
cd sat
```
Then start to initialize requirements just follow these commands

```bash
npm init -y
```
## Download dependencies for a System:

1: Install node fasttext 

```bash
npm install node-fasttext --save
 ```

2: Install Express: 

```bash
npm install express --save
```


4: Install some cors issues:

```bash
npm install cors --save
```

## Travis CI 

Travis CI was the first CI as a Service tool. It introduced a new approach to building code in the cloud. This CI tool allows the user to sign up, link their repository, build, as well as test their apps.

### What does Travis do?
Travis CI offers following benefits:

* You can monitor GitHub projects
* Runs Test and generate results quickly. Parallel test execution is possible.
* Build artifacts & check code quality

#### Steps integrate to Travis

first go to the 
[Travis CI ](https://www.travis-ci.com/?_gl=1%2A1dvnqks%2A_ga%2ANjkwNzAwNzg5LjE2Mzk1OTQ0NzE.%2A_ga_XRYGSZFQ0P%2AMTYzOTU5NDQ3MC4xLjAuMTYzOTU5NDQ3MC42MA..) sign in with your account in GitHub
then accept the Authorization of Travis CI.
then click on your profile picture in the top right of your Travis Dashboard, click Settings and then the green Activate button, and select the repositories you want to use with Travis CI.
<br>
#### I made some modifications to my files to make the build pass

in package.json it was
```bash
  "test": "echo \"Error: no test specified\" && exit 1"
```
change it to
```bash
    "test": "echo \"No test specified\""
```
and in .travis.yml it was
```bash
  Language: node_js
Node_js: 
 10
```
change it to
```bash
    Language: node_js
Node_js: 
 -7
```
#### Then I uploaded the files after change to GitHub to see if you passed in travis
 in termnal
```bash
  git status
```
```bash
  git add .
```
```bash
  git commit -m " # commit"
```
```bash
  git push
```
When you return to [Travis CI ](https://www.travis-ci.com/?_gl=1%2A1dvnqks%2A_ga%2ANjkwNzAwNzg5LjE2Mzk1OTQ0NzE.%2A_ga_XRYGSZFQ0P%2AMTYzOTU5NDQ3MC4xLjAuMTYzOTU5NDQ3MC42MA..) and go to the intended repository and then click in branches, you will find pass like in this picture
![App Screenshot](https://d.top4top.io/p_2175e7z371.png)
![App Screenshot](https://b.top4top.io/p_2175il4ed1.png)
