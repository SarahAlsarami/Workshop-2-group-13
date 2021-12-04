
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

## Run Node.js 

```bash
node index.js
```

## Screenshots of the output

![App Screenshot](https://e.top4top.io/p_2163rj97k1.png)

now when I go to a file "index.html" and open it
 in the browser


![App Screenshot](https://g.top4top.io/p_2163ulhw82.png)

and when he writes anything, it gets classification 

![App Screenshot](https://l.top4top.io/p_216377f7g3.png)

Success will appear and then return to the terminal

![App Screenshot](https://f.top4top.io/p_2163glgi51.png)
![App Screenshot](https://k.top4top.io/p_2163ov1891.png)


## Appendix

how to install virtualbox and Ubuntu :

https://youtu.be/x5MhydijWmc
