![gws_logo](https://github.com/shareme/EDroidClassic/raw/master/readme_images/grottworkshop_logo.png)
EDroidClassic
---

Eclipse Classic Android project layout before the Google ADT plugin fully suppports  gradle builds.
Its not a pernament thing as I expect ADT version 23.x with full gradle support to be released in
mid Summer 2014.

# Best Practices

* Parent container keeps a sane naming method corresponding with the repo name.
* Gradle cannot handle side-by-side sub-projects so we nest with parent app first and than
  the test app and also the set of AndroidProjectLibraries.

# Quirks

Yes, you have to remember to navigate to the separate project folder of sub-project in the left naviagtion
pane showing package explorer any time you want to do anything project related, but I am used to eclipse
and I am not switching.

Yes, you have to convert each sub-project to gradle and yes you will have to re-assign the gen and src inputs as the
conversion to gradle messes them up as of Eclipse 4.3.

In Eclipse Classic Android gradle layout we do not test APLs except by test app coupled to the parent app.

# Handling Multiple APLs with different IDEs with different project layouts or build systems(maven).

Right now, Eclipse ADT 22.x does not handle AARs. That means that whatever 3d party APLs you are using
you will have to find a way to integrate those with your gralde builds. THe best way to do that is yo are creating
a sub-project folder that will contain the git repo module if you are daring. I say daring because that couples your
project to that 3d party APLin that its changes will appear right away in your project.

But there is a hack way to do this. Fork third party APL on your git host like github or bitbucket, etc. Than use that fork
as a git module as will be current as the date of the fork. To do this right adapt a naming strategy for the
forks. This way you will not tightly couple your app to the APL.

After a while of using 3d party APLs you will start to notice certain ones using gradle-maven-idea or
gradle-idea,etc  You can make up templates in gradle that convert the Eclipse classpath to have the right structure
of sub folders,etc.

# Usage

Just open up the Eclipse IDE and mirror the nested project folders for youru android application.

# License

Copyright 2014 Fred Grott GrottWorkShop

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

<a href="http://www.apache.org/licenses/LICENSE-2.0" rel="license">http://www.apache.org/licenses/LICENSE-2.0</a>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


# Development Resources

As always Google Engineers and OEM Engineers do not answer direct android
application development questions by emial and so these resources are
somewhat better to use for that purpose.

<a href="https://plus.google.com/u/0/communities/105153134372062985968">G+ Android Application Development Circle</a>
<a href="https://plus.google.com/u/0/communities/113499773637471211070">G+ Android Design Circle(private invite only</a>
<a href="http://stackoverflow.com/questions/tagged/android">Stackoverflow Android Area</a>



# About The Author

Fred Grott is an Android Application Engineer that develops android applications
for startups and firms in the Greater Chicago area. His encyclopedia of android
internals and android techniques combined with expert java and computer science
skills and knowledge make short work of tough and challenging development
problems for firms in the Greater Chicago area everything from mobile web applications
to hybrid mobile web and native applications and all the way to android native applications.

Being an Agile Rockstar Android Developer means Fred Grott uses expert java techniques to
choose what methods are effective to solve specific problems. For example, annotations
performance is not robust enough just yet to fully use dependency injection to separate
concerns so modifying MVC into Passive MVC is used to separate concerns such as business logic,
views, and model.

He can be followed on many of his Social Profiles:
<a href="http://goo.gl/M0o50J" rel="me">About.me</a></br>
<a href="http://goo.gl/EmChpW" rel="me">AngelList</a></br>
<a href="http://goo.gl/sEmqJr" rel="me">Behance</a></br>
<a href="http://goo.gl/Mg8r1w" rel="me">BitBucket</a></br>
<a href="http://goo.gl/84p6gA" rel="me">CoderBits</a></br>
<a href="http://goo.gl/lbdx0x" rel="me">CoderWall</a></br>
<a href="http://goo.gl/uun5Qg" rel="me">DeviantArt</a></br>
<a href="http://goo.gl/Vt06L1" rel="me">Dribbble</a></br>
<a href="http://goo.gl/aECSjf" rel="me">Forrst</a></br>
<a href="http://goo.gl/ky9TYK" rel="me">GeekList</a></br>
<a href="http://goo.gl/8wT7LJ" rel="me">GitHub</a></br>
<a href="http://goo.gl/hls95u" rel="me">Gitorious</a></br>
<a href="http://goo.gl/Whf9u3" rel="publisher" rel="me">G Plus</a></br>
<a href="http://goo.gl/2W9e0U" rel="me">HackerNews</a></br>
<a href="http://goo.gl/wCXLYC" rel="me">Html5Ninja</a></br>
<a href="http://goo.gl/7EAFvt" rel="me">LinkedIN</a></br>
<a href="http://goo.gl/sXAS4C" rel="me">MasterBranch</a></br>
<a href="http://goo.gl/xl5cHu" rel="me">Reddit</a></br>
<a href="http://goo.gl/cxs3I2" rel="me">Quora</a></br>
<a href="http://goo.gl/WnemaH" rel="me">SlideShare</a></br>
<a href="http://goo.gl/8y8HDI" rel="me">SpeakerDeck</a></br>
<a href="http://goo.gl/A03BmA" rel="me">StackOverflow</a></br>
<a href="http://goo.gl/TrPn9r" rel="me">ThemeForrest</a></br>
<a href="http://goo.gl/J3dnsA" rel="me">Twitter</a></br>
<a href="http://goo.gl/83Z9aC" rel="me">Udemy</a></br>
<a href="http://goo.gl/kO7g5i" rel="me">YouTube</a></br>

His main websites are:
<a href="http://grottworkshop.blogspot.com/" rel="me">Blog at Blogger</a></br>
<a href="http://goo.gl/ReBZKD" rel="me">GWS site at Github.io</a></br>
<a href="http://goo.gl/D9lo1D" rel="me">AndroidHacker</a></br>

# Contacting Author

The author can be contacted by visiting these profiles and
using the contact links:
<a href"http://goo.gl/M0o50J" rel="me">About.me Profile<a></br>
<a href="http://goo.gl/Whf9u3" rel="me">Google Plus Profile</a></br>

# Endorse The Author

[![endorse](https://api.coderwall.com/shareme/endorsecount.png)](https://coderwall.com/shareme)