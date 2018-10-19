# What is the A/B Testing?
AB testing is a type of experimentation that helps to compare two different versions of a web page to check which one has more clicks or visitors. 

# Project:

For this project, I am working on to understand the results of an A/B test run by an e-commerce website.
The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product.
The goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

##### The Goal to Complete the project:
  
  - Answers to the questions
  - Code to solve the problems 
  - Comments when necessarary

##### Another Files in Analyze-A-B-Test-Results:
  - "ab_data.csv" and "countries.csv" are files that consists of data and used as to data analyzation. 
  - "Analyze_ab_test_results_notebook_original.ipynb" is the file project, written in python and jupyter notebook
  - "Analyze_ab_test_results_notebook.html" can be display in html

### 

Analyze-A-B-Test-Results uses a number of open source projects to work properly:

* [Jupyter Notebook] or [Python] - jupyter notebook is an open source and used to data analyse with python code
* [matplotlib] - uses to faciliates the data analyzation by displaying the plots
* [numpy] - is a fundamental scientific computing.
* [Pandas] - uses to clean, organize, convert, and merge the data.

### Installation

Analyze-A-B-Test-Results requires anaconda and jupyter notebook [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| Github | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantanously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT

