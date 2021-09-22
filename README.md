# Digital research methods for textual and network data: Resources and tools {-}
<!-- Last update: October 8, 2020 (17:30) -->
_Author: Jay Lee_  
_Last update: Sept. 21, 2021 (18:56)_

# Table of contents {-}

1. [Preliminary instructions and caveats](#preliminary-instructions-and-caveats)
2. [Preparation for Week 1](#preparation-for-week-1)
3. [Zoom and meeting schedule](#zoom-and-meeting-schedule)
4. [Weekly slides and data](#weekly-slides-and-data)
5. [Resources and readings](#resources-and-readings)
6. [Detailed preparation](#detailed-preparation)
7. [Software tools](#software-tools)

---

# Preliminary instructions and caveats
1. There are various download and hyperlinks throughout this documents. These should appear in <span style="color:royalblue">blue</span>.
   - I recommend right-clicking and opening new links in a new browser tab.
2. Link for this document is [https://bit.ly/drm_phd_instructions](https://bit.ly/drm_phd_instructions) .
   - You will have to open this document in a web browser.
   <!-- - You should be able to navigate around this document directly on Dropbox, but you're free to also download it and view it locally. -->
   - I'll be updating this file throughout the course with links to new material, so keep this link handy somewhere.  
<!-- [https://bit.ly/phd20_html_instructions](https://bit.ly/phd20_html_instructions) -->
<!-- https://www.dropbox.com/s/wqpvaa0pr8iqqic/DRM_PhD_course.html?dl=0 -->
<!-- https://bit.ly/3EFNgXN -->
<!-- https://bit.ly/3nVfwjs -->
3. If for some reason an external link in this document does not work, just copy the URL (right-click, copy) and then paste it into your web browser.
4. Please contact me first, if you have any intention of sharing the course material with others not in the course :-).

## Caveats

Here are three technical points that trip up some students every year.

1. [**ZIP archive**:]{.ul}
   * Some of the tools and data you download will come in the form of a `.zip`, or ZIP file/archive.
   * These are archive/packages that do not automatically install.
   * You need to double-click on the file (from Windows Explorer or Mac Finder), **but then** you need to copy out (aka extract) its contents to somewhere like Documents or Downloads.
   * That is, programs do not run properly from within a ZIP archive nor can data within a ZIP be loaded.
   * It's easiest to just copy out the top level folder within the archive and everything under it will copy along.
2. [**CSV file** and the dreaded comma:]{.ul}
   * Many of the data in this course will come in the form of a `.csv`, or CSV file (aka comma-separated-value file).
   * These are simple text files that are meant to be open as tabular data, like in Excel.
   * So, it employs a character (usually comma) to distinguish one column from another.
   * However, in Europe, Excel expects a semi-colon, while many tools expect a comma. There are instructions below on how to deal with this.
3. [**Best computer** to use for course:]{.ul}
   * Because using software, esp. free scientific software, sometimes incurs technical issues, here is an ordering from the least problematic computer type to the most:
   a. Least complicated: _personal Windows laptop_
      - Assumes you have full rights to install software.
      - However, if your laptop's default language is not English, you could run into some issues with some of the course tools.
   b. Some minor complications: _EUR pclab desktop_
      - The only hurdle with this is a few extra steps required to access some of the course tools.
   c. A few more complications: 
      i. _personal Mac laptop_
         - There is no Mac version for one of the course tools and some MacOS versions can be cranky with some of my custom scripts.
      ii. _EUR office desktop_
          - You would have to install some course tools from the Software center and also take a few steps to access some of the other tools from the EUR server.
      iii. _EUR laptop_
           - Because of restricted rights to install programs, people in the past had installation issues.
           - If you have to use an EUR laptop, contact EUR IT to see if you can be granted "local admin" rights for user account in the laptop.
   
_[Click here](#table-of-contents) to jump back to table of contents._

---

# Preparation for Week 1

_See the [Software tools](#software-tools) section for download links and license._

1. Download and install the Tableau program:
   1. Optional: Suggest some hashtags in this [Google Doc](https://bit.ly/2RqXtjV) for us to analyze before class. I'll need to download these ahead of time.  
   **OR**
   2. Optional: Use Tableau to obtain your own tweets (see pre-release Week 1 Hands-On slides)
   * Both of the above are optional before class.
2. Install ConText:
    1. Download and unzip Parse Nexis (zip)
    2. Download and install ConText (installer).
3. If you have your own text documents that you'd like to analyze, email them to me (or let me know about them) and we can see about how you can use them in the course.
4. Read the Week 1 readings (but you can skim the DRM SG readings as they're supplemental). See [Resources and readings](#resources-and-readings).
5. Read through all of the [Detailed preparation](#detailed-preparation) section of this document.

_[Click here](#table-of-contents) to jump back to table of contents._

---

# Zoom and meeting schedule

[Link for all Zoom meetings](https://eur-nl.zoom.us/j/91909873219)
* Also, you should have already received the Zoom link via email.

<!-- https://eur-nl.zoom.us/j/98472445726?pwd=dWQzay9CVFJUd0E3R1p1Q1U4cHQyZz09) -->

<u>Class times (all on Friday):</u>

|Week| Date| Time |
|:--:|:--|:--:|
|1| September 24, 2020 | 09.30-12.30
|2| October  1, 2020 | 09.30-12.30
|3| October  8, 2020 | 09.30-12.30
|4| October 15, 2020| 09.30-12.30

_[Click here](#table-of-contents) to jump back to table of contents._

---

# Weekly slides and data
* _PDF slides will be made available just before or during class._
* _For any of the PDF links, you may view them comfortably on Dropbox/web browser, or you can download them (click on the "..." icon if you don't see a Download icon)._

## Week 1

Week 1 - Twitter, visualization in Tableau and text analysis in ConText

* [Week 1 lecture](https://bit.ly/phd_lecture_1)  
  <!-- https://bit.ly/3nRuV42 -->
* Week 1 hands-on: [1a](https://bit.ly/phd_hands1a) (pre-release) and [1b](https://bit.ly/phd_hands1b)  
  <!-- https://bit.ly/3Aswida, https://bit.ly/3lOrF7b -->
  - For now, 1a is a pre-release (subset of full slides) for those who want to try downloading Twitter data via Tableau before class.
  - It will be the full version on Friday.
  - You can make use of the internal links in the pdf slides to help you navigate.
  - From Dropbox, you can also download the PDF to your own computer, if you prefer.
* [Week 1 data](https://bit.ly/phd_data1) (ZIP file)  
* Both hands-on (will) have instructions for connecting an EUR computer to the EUR server in order to run some course programs. These include ConText, Parse Nexis, Mozdeh and SentiStrength.
  * Those instructions may also work for the EUR laptop (if you don't have local admin privileges to properly install software).
  * <u>For an EUR laptop:</u>
  * Try the connection without EduVPN first; it works for me without EduVPN.
  * Under this approach (as opposed to installing the software on the computer), it will take a bit longer for a laptop to load in programs as it has to communicate over the internet (i.e., a few minutes to bring up ConText, several seconds for Mozdeh).
<!-- * For some reason, Tessa was unsuccessful with this when trying from outside EUR; it works for me (both at home and at EUR). -->
<!-- * Alternative slide links for Week 1 (use these only if the above links do not work for you): -->
   <!--   * [Lecture](https://www.dropbox.com/s/79m1lxobrlwsl2d/DRM_PhD_Week1_Lecture.pdf?dl=1) -->
   <!-- 	   ; [Hands-On 1a](https://www.dropbox.com/s/ew974vm14k90hm0/DRM_PhD_Week1a_Hands-On.pdf?dl=1) -->
   <!-- 	   ; [Hands-On 1b](https://www.dropbox.com/s/imieda4daze21lx/DRM_PhD_Week1b_Hands-On.pdf?dl=1) -->
   <!-- 	   ; [Data](https://www.dropbox.com/s/p9p7sjonlgre9ux/DRM_Week1_Data.zip?dl=1) -->

## Week 2

_Material for later weeks will be added to this HTML document._

_[Click here](#table-of-contents) to jump back to table of contents._

---

# Resources and readings
* <a name="sg"></a>[Digital research methods: Step-by-step guide](https://bit.ly/drmsg_noneshcc) (aka **DRM SG**)  
<!-- https://www.dropbox.com/s/paqmp1kb5hn99ow/DRM_Step_by_Step_Guide_nonESHCC_Lee_Latest.pdf?dl=0 -->
  * While the practical, hands-on portion of the course will rely on explicit step-by-step slides, the DRM SG has some additional steps and material, not covered in those slides. It's just good to keep this handy.
* <u>Readings:</u> 
  * _The reading links below will directly get you the article._
  * _For any of the DRM SG readings, you can just skim the explicit steps (i.e. just familiarize yourself with the description of the tool or method or any issues discussed)._
* Readings for _Week 1_:
  * _Just familiarize yourself with_:
    - DRM SG, sections on 1, 1.1-1.4. section 3 (intro part only, before 3.1)
    - DRM SG, sections 4.2-4.3, 4.5, 4.6
  * Levallois, C. (2017). [A primer on text mining for business](https://seinecle.github.io/mk99/generated-pdf/text-mining-for-business.pdf). Online.
* Readings for _Week 2_:
  * DRM SG, sections 4.8, 5
  * Blei, D. (2012). [Probabilistic topic models](https://bit.ly/2RJnaMx). _Communications of the ACM_, _55_(4), 77-84. (Focus on the sections leading up to ‘LDA and probabilistic models’)
  * Thelwall, M. (2017). [Heart and soul: Sentiment strength detection in the social web with SentiStrength](http://sentistrength.wlv.ac.uk/documentation/SentiStrengthChapter.pdf). _Cyberemotions: Collective Emotion in Cyberspace_, 119-134. (Paper also available on SentiStrength website; focus on sections Introduction, Using, Core, Additional,Sarcasm, Application; you may skim the rest)

* Readings for _Week 3_:
  * DRM SG, section 6 (up through 6.8)
  * Levallois, C. (2017). [A primer on network analysis for business](https://seinecle.github.io/mk99/generated-pdf/network-analysis-for-business.pdf). Online.
  * _Optional for background on network analysis:_
  * Borgatti, S. P., Mehra, A., Brass, D. J., & Labianca, G. (2009). [Network analysis in the social sciences](https://bit.ly/2RLdRvB). _Science_, _323_(5916), 892-895.
  * Hanneman & Riddle (2005). [Chapter 1: Social network data](http://faculty.ucr.edu/~hanneman/nettext/C1_Social_Network_Data.html). [_Introduction to Social Network Methods_](http://faculty.ucr.edu/~hanneman/nettext). Online.
* Readings for _Week 4_:
   * DRM SG, sections 6.9, 7.1, 7.2, 7.3

_[Click here](#table-of-contents) to jump back to table of contents._

---

# Detailed preparation

## Warning: European or U.S. regional settings on your laptop

Most of the tools of this course rely on the commas' not being used as the decimal (and rather the period). However, the comma as decimal is common in Europe and is often the default setting for laptops purchased in Europe. Just keep this in mind OR you can check/change this setting on your laptop. See section F.1 of the [DRM SG](#sg) for instructions on dealing with this issue, for when you encounter the problem.

## Your own data (optional)
Remember you are welcome to use your own data for many of the activities in the course. 
* Any non-text files (like DOCX or PDF) will have to be converted into "text files"; I can assist with this.
* A "text file" is like a Word document, but much more simplified, containing only basic letters, numbers, and punctuation.
* Also, these can be easily saved/export from Word or Adobe Acrobat PDF.
* The default program for opening text files (i.e. double-clicking on it) is usually not Word or Adobe. Instead: Notepad for Windows and TextEdit for Macs.
* An unstructured text file (i.e. not a CSV) usually has the file extension `.txt`.

_Contact me if you encounter difficulties converting/saving your data as text files._

_[Click here](#table-of-contents) to jump back to table of contents._

## Week 1's Twitter data: A request for \#hashtags (optional)

We'll scrape Twitter data in Week 1 to explore features of the tool Tableau. However, the Twitter scraping engine of Tableau has some limitations, such that we may not all be able to successfully scrape at the same time during class. For this reason, I ask you to anonymously offer some hashtags - on a topic of your interest - in this [Google Doc](https://bit.ly/2RqXtjV). I'll try scraping data for some of them before our first meeting.
<!-- * _Forthcoming: I'll update this document soon with some instructions for you to download Twitter data through Tableau, so that you can do so on your own before our class meeting._ -->

_[Click here](#table-of-contents) to jump back to table of contents._

## Tools

<u>Your own or EUR laptop:</u> If you are using a laptop to follow the course, please install the [tools](#software-tools) below (at least the ones needed before each week's meeting).

<u>EUR pclab:</u> If you are using an EUR pclab computer, the Week 1 hands-on slides have instructions on how to run the tools. You do not need to download anything.
* Tableau and Gephi are already installed in all pclabs.

<u>EUR office desktop:</u> If you are using an EUR office desktop that is not in a pclab, you should be able to install Tableau and Gephi onto the desktop from the Software Center (I'm not 100% sure about this). For the other tools, you'll have to follow the instructions in the slides to access the EUR servers, just as if you were in a pclab.
* It might be possible to install software into Documents/NO-APP-CONTROL.

### <u>WARNINGs for EUR computers</u>
* For those of you with EUR-maintained computer (i.e. laptop or office desktop), if your installation for any of the tools fails or fails to run (after you install in the default folder suggested by the tool), you have a few options:
* The tools may install (or unzip) to Documents/NO-APP-CONTROL.
* You can ask IT for "local admin privileges"; this way you can install programs under the "Program Files" folder.
* Two of the tools (Gephi and Tableau) are available from the Software Center.

_[Click here](#table-of-contents) to jump back to table of contents._

---

# </a>Software tools

<a name="tools">
As this is a non-programming course, we rely GUI tools (GUI=graphical user interface). Unfortunately, DRM is a complicated domain, and so there is no single GUI tool that accomplishes all of the DRM covered in this course. Thus, we must avail ourselves of several different tools. All of the tools are downloadable using the links on this page.

If you are interested in the programming route - which, for this course, doesn't actually require too much programming knowledge/skill, you are welcome to use 'R', an open source statistical computing program that is widely used in data science. The R route can replace most of the text analysis components of the course. The software below that can be replaced by R will show `(also in R)` by its title. For R, jump to [Instructions for R](#r_instruct) (in this document).

For any of the ZIP archive downloads, you will need to copy/extract out its contents (usually just the top level folder in the archive) to somewhere on your laptop. That is, you shouldn't run the program but double-clicking on the ZIP file and then double-clicking again program (showing within the ZIP program).

_[Click here](#table-of-contents) to jump back to table of contents._

## Week 1

You'll need these tools starting from our first class meeting and also for some of the subsequent meetings.

### Tableau

Tableau is a general-purpose, (semi-)intuitive data analytics and visualization application. We will use this program to 1) download some Twitter data and 2) visualize some of the quantitative outputs.

Use one of the links below to download Tableau.

* [Tableau 2020 1.8 for Windows](https://bit.ly/33yeZbi)
* [Tableau 2020 1.8 for Mac](https://bit.ly/2FF8fAj)
  * According Tableau, the Mac version will work only on macOSes High Sierra 10.13, Mojave 10.14 and Catalina 10.15.
  * _If you have an older macOS, this version still may work. If it does not, contact me and we can try an older version._

<!-- 1. You will need the student license, which expires on Oct 23, 2020: **TC0B-AA82-66C0-4A36-E53B** -->
1. You will need the following student license: **TC60-4600-DEF0-17A5-3C0F**
   * Use this only for a laptop or an EUR office desktop.
   * If you see an expiration message on an EUR pclab desktop, please let me know before using this license.
2. You are welcome to use the latest version of Tableau from their website (version 2021.3). However, some of the hands-on steps will be different for you, than what appears on the hands-on slides, which have been tailored for Tableau 2020 1.8.
3. If you like Tableau, you can apply for a full one year student license through their website.

* For more information on Tableau: [tableau.com](https://tableau.com)

### Parse Nexis

In order to quickly transform downloaded LexisNexis articles into text files, we need a separate parsing tool (that I wrote). Parsing LexisNexis articles can be done in `R`.
* [Parse Nexis for Windows](https://bit.ly/3evYuRG)
* [Parse Nexis for Mac](https://bit.ly/2ViaI8U)

### ConText
ConText is a general purpose text analysis tool. Text analysis can also be done in `R`.
* [ConText 1.2.0 for Windows](https://bit.ly/2XLq3R9)
* [ConText 1.2.0 for Mac](https://bit.ly/2XKXjI5) (will not work for Catalina/Big Sur)
* [ConText 2.0 for Mac (Catalina/Big Sur)](https://bit.ly/35L1est)
  * This beta version works for the latest Mac OSX.
  * It should work for older versions too, but 1.2.0 is a bit more stable.
* [ConText 2.0 of Java 8](https://bit.ly/context_2_java)
  * This version should be runnable from an EUR laptop (without local admin privileges) or the EUR pclab.
  * For an EUR laptop, you need to install Java 8 from the Software Center. See the README file of the ZIP archive.
<!-- * [ConText 2.0 for Mac Catalina](https://bit.ly/2Y5fg4v) -->

If ConText does not install properly at first, you should try to install with Administrator privileges:

* Windows: Right-click on the installer and choose Run as Administrator
* Mac OSX:
   * Go to: _System Preferences → Security & Privacy_:
     * If needed, click on "Click the lock to make changes"
     * Select "Allow apps downloaded from:"
     * Change that to: "App Store and identiﬁed developers"

* For more information on ConText: [context.ischool.illinois.edu](http://context.ischool.illinois.edu/)

_[Click here](#table-of-contents) to jump back to table of contents._

---

## Week 2

### SentiStrength `(in R)` (Week 2, optional)
SentiStrength performs more accurate sentiment analysis than the sentiment analysis facility in ConText.
* [SentiStrength 2.3 for Windows](https://bit.ly/355vN9M)
* [SentiStrength 2.3 for Mac](https://bit.ly/2xZorIP)
  * The Mac version is not quite a GUI but script driven.
  * It requires a few (easy) manual steps. See the section 5.2.2 in the [DRM SG](#sg).
  
* For more information on SentiStrength: [sentistrength.wlv.ac.uk](http://sentistrength.wlv.ac.uk/)

_[Click here](#table-of-contents) to jump back to table of contents._

---

## Week 3

### Gephi

Gephi is a general purpose network analysis tool.

* <u>Your own laptop:</u>
  * [Gephi 0.9.2 for Windows](https://bit.ly/2WgzyX6)
  * [Gephi 0.9.2 for Mac](https://bit.ly/2zivNaO)
  * You're welcome to download either from the Gephi website. However, for Windows, you should already have Java installed. My ZIP package includes a local version of Java (i.e. it won't interfere with your already-installed Java, if that's the case).
* <u>EUR laptop or office desktop:</u>
  * Install Gephi 0.9.2 from the Software Center.
* <u>EUR pclab:</u>
  * Run Gephi from pclab computer; it's already installed.
* For more information on Gephi: [gephi.org](https://gephi.org)

_[Click here](#table-of-contents) to jump back to table of contents._

---
## Other optional tools:
### SNScrape

I used to offer a GUI tool - GetOldTweets - that would let you easily scrape tweets that are more than a week old. However, due to Twitter's changing policies, this tool no longer works. There is an alternative tool I offer called SNScrape that still works. However, it's slightly trickier to use. [Click here](html/snscrape.md) to see full download and usage instructions.  
<!-- https://www.dropbox.com/s/r5jzvzj417y9mz5/SNScrape_for_PhD.html?dl=0 -->
<!-- https://bit.ly/3Auu1hy -->

### Mozdeh
Mozdeh performs API-based Twitter scraping similar to Tableau, meaning it is good for scraping lots of tweets that have occurred in the last week (or up to 3500 tweets from a specific username with no time limitation).

Unfortunately, Mozdeh is available only for Windows. Mac users would have to run this program within a virtual environment (e.g., VirtualBox, Parallels, etc.)
* [Mozdeh for Windows](https://bit.ly/2zcyFWI)
  * Mozdeh will require you to log in to Twitter during its use, so you will need to have your Twitter login information handy.
  * It only needs your login credentials to assign you temporary access to Twitter's API. As far as I'm aware, there is no privacy/security risk.
* For more information on Mozdeh: [http://sentistrength.wlv.ac.uk/](http://sentistrength.wlv.ac.uk/)

### Parse Facebook

The Parse Facebook tools assists in your acquiring posts from either public FB _**pages**_ or a _**search**_. There is some manual labor required on your part (scrolling through a feed and then copy-pasting its contents).

* For posts on a page, download [Parse Facebook 2020](https://bit.ly/parse_fb_2020)
  * Then, see section 2.3.5 of the [DRM SG](#sg) for explicit instructions
  * _This script may no longer work with the new post-Sept-22nd Facebook layout._
* For posts from a search, download [Parse Facebook Posts 2020](https://bit.ly/parse_fb_posts)
  * This one works only with the post-Sept-22nd Facebook layout.
  * See the README.html within the downloaded zip for more information.

_[Click here](#table-of-contents) to jump back to table of contents._

----

### <a name="r_instruct"></a>Instructions for R
* [Instructions for R](https://bit.ly/2ysfCqQ)
* [Dropbox tools/R folder](https://bit.ly/3c99a7V){target="_blank"}
