# sense-extension-install

> Some instructions & FAQs to install extensions for Qlik Sense.

---

## Table of Contents

- [About](#about)
- [Download the Extension](#download-the-extension)
- [Installing Qlik Sense Extensions](#installing-qlik-sense-extensions)
  * [Installing on Qlik Sense Desktop](#installing-on-qlik-sense-desktop)
  * [Installing on Qlik Sense Server](#installing-on-qlik-sense-server)
- [FAQ](#faq)
  * [I am getting error XYZ](#i-am-getting-error-xyz)
  * [I am getting an error uploading the extension to Qlik Sense Server, what can I do?](#i-am-getting-an-error-uploading-the-extension-to-qlik-sense-server-what-can-i-do)
  * [Why can't I just download the GitHub project?](#why-cant-i-just-download-the-github-project)
- [About](#about-1)
  * [Author](#author)

_(TOC generated by [verb](https://github.com/verbose/verb) using [markdown-toc](https://github.com/jonschlinkert/markdown-toc))_

---

## About

The instructions below will help you to install extension **I (Stefan Walther)** have created. All Qlik Sense extensions I have created, follow the same rules.

__Note: Other authors might very likely follow different approaches.___

## Download the Extension

I structure all extensions the same way. GitHub is used to host the source code, but also different builds of the extension.  

If you want to start using one of my extensions in either Qlik Sense Desktop or Qlik Sense Enterprise, please consider:

- There is a folder called `build`. 
  - This folder typically contains several versions of an extension, each of them packaged as .zip file.
- Download the file called `%extension-name%_latest.zip` resp. the version you want to download.
- Follow the instructions below

## Installing Qlik Sense Extensions

### Installing on Qlik Sense Desktop

Follow the instruction [here](http://help.qlik.com/en-US/sense-developer/September2017/Subsystems/Extensions/Content/Howtos/deploy-extensions.htm).

### Installing on Qlik Sense Server

Follow the instructions [here](http://help.qlik.com/en-US/sense-developer/September2017/Subsystems/Extensions/Content/Howtos/deploy-extensions.htm).

## FAQ

### I am getting error XYZ

First of all don't do download the entire GitHub repository, this is the most common mistake.

![](./docs/images/dont-github-download.png)

You are then downloading the entire GitHub repository, containing (potentially) multiple versions of an extensions.  
Importing the resulting .zip file will fail when importing in Qlik Sense.

**Resolution:** See [here](#download-the-extension)

---
### I am getting an error uploading the extension to Qlik Sense Server, what can I do?  

As you upload a .zip file to Qlik Sense Server I first recommend to unzip the file locally to have a look into the content of the .zip file:

- You should see a .qext file at the root of the .zip file's content
- See [here](#download-the-extension)

---
### Why can't I just download the GitHub project?  

I have structured all my extensions in the same way:

- There is a `./build` directory where you can download multiple versions of an extension.

If you download the entire GitHub repository, it will contain most likely multiple .zip files containing a specific version of an extension.  
The solution is simple: Go to the `./build` directory and download the desired version, by default the go for the file `%extension-name%_latest.zip

## About

### Author
**Stefan Walther**

* [twitter](http://twitter.com/waltherstefan)  
* [github.com/stefanwalther](http://github.com/stefanwalther) 
* [LinkedIn](https://www.linkedin.com/in/stefanwalther/) 
* [qliksite.io](http://qliksite.io)

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.6.0, on February 09, 2018._

