![Angry Jenkins Logo](https://github.com/10000TB/Jenkins-Plugin-Examles/blob/master/not-examples-related/ninjenkins.svg)  
# Jenkins-Plugin-Examles
This is a collection of Jenkins plugin examples, which could be a great start point for getting started with developing Jenkins plugin. 
  
  
[Usage](#usage)  
[Useful readings](#reading)  
[Wishlist](#wishlist)  
[Motivation](#motivation)  
[Contribute or Request a new example](#contribute-or-request-a-new-example)  
[Acknowledgement](#acknowledgement)  
[Categories](#category)  
* [Develop a new step in Groovy pipeline](#develop-a-new-step-in-groovy-pipeline)

## Usage
To see how the plugin works, simply run
```
mvn hpi:run
```
you will be able to see how each plugin works on a local live Jenkins server.  
Then checkout the classes, and supporting files and understands how the plugin comes together.  
  
It is suggested that you go through all examples in the list before you can write your own plugin. Simply go through some of them, and then focus on those examples related to your needs.

## Reading
* [Best Practices for Scalable Pipeline Code](https://jenkins.io/blog/2017/02/01/pipeline-scalability-best-practice/)

## Wishlist
* Split big plugins into smaller examples demonstrating how each small functionality is implemented.

## Motivation
When I first started looking at how to develop a Jenkins plugin, I spent quite some time on searching for useful education materials online. Despite the fact that there is ton of docs online that guide you on how to develop a Jenkins plugin, I often find that **playing with some basic examples of a new thing(plugin here)** can quickly bring you up to speed to work on it in a productive way. As a result, I didnt find any place providing such list of examples, and to embrace the spirit of open source, I am opening up this repo with some of the examples I used in learning developing Jenkins plugin. I hope that this will serve as a base for a complete list of basic examples that cover most Jenkins extension points. So, feel free to contribute any new basic example plugin that covers uncovered Jenkins extension points. Cheers!   

## Contribute or Request a new example  
If you find that the following list (in `Category` section) is missing an example of such plugin where Jenkins can be extended. Feel free to contribute an example, or open a new issue to request an example.

**Contribution Guide**:  
* Be sure about what you are contributing!  
  * Avoid duplicate
  * Adding a directory means you are opening a new plugin category
  * Adding an example under existing directories means you are adding an example for that category
* Make it work before submitting a PR
  * It is always frustrating to present new developers with sth not working! So better make it work before a PR :)
* Make it simple
  * This project is meant to bring new developers into plugin development, so make things simple and concise

## Acknowledgement
Many of the starting examples I put in the list here are directly referenced from their repos on github. Here, I am only doing some commenting, and organizing work to put them together so it is easier for beginners read and learn. Since there are too many of them, I am not doing a creditting accounting here, but simply acknowledging all of them here in this section.

## Category

##### Develop a new step in Groovy pipeline
Checkout directory: `workflow-basic-steps-plugin`  
Representative implementations:  
`echo` step: `Jenkins-Plugin-Examles/workflow-basic-steps-plugin/src/main/java/org/jenkinsci/plugins/workflow/steps/EchoStep.java`  
`pwd` step: `Jenkins-Plugin-Examles/workflow-basic-steps-plugin/src/main/java/org/jenkinsci/plugins/workflow/steps/PwdStep.java`  

(todo:10000tb) add links for example ui plugins, builder plugins.

## Liscense

State-replay is under [MIT Liscense](https://github.com/10000TB/Jenkins-Plugin-Examles/blob/master/LICENSE), The terms of the license are as follows:

```
MIT License

Copyright (c) 2017 Xuehao(David)  Hu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
