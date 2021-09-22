### Get older tweets using SNScrape 
_Last update: May 3, 2021 (15:14)_

* SNScrape allows you to scrape tweets older than 1-2 weeks.
  - In fact, it lets you get (a sample) of tweets at any point in time, since the founding of Twitter in 2006.
* In previous years, we used a tool called GetOldTweets to acquire old tweets. But, due to Twitter API/policy changes, this tool no longer works.
* A newer tool called SNScrape will scrape this.
  - The SNS part refers to SNS or social networking sites.
* It might be tricky to use for some of you, and unfortunately there's no GUI (graphical user interface) for it yet.
* I've named the version we're using as `snscrape36`.
  - Technical note: the `36` refers to Python 3.6 that was used to package the tool.
  - Also, note that when running the tool, it's entire name is lower-cased: `snscrape36`.
* Click on one of the links here to jump to the appropriate subsection on this page: [Windows](#snscrape_windows) or [Mac](#snscrape_mac)
* Also, **don't forget** to look at [Final notes](#snscrape_final).

### <a name="snscrape_windows"></a>SNScrape for Windows
1. [Click here](https://bit.ly/3umpknl) to download the tool (a ZIP file)
   - Copy the top-level `snscrape36` folder out of the ZIP, e.g., Downloads or Desktop or wherever, just remember where you put it.
   - For Windows, depending on your user account's security settings, you may want to copy this into `Program Files`.
1. Open the Command Prompt program (search for "CMD")
2. Now you need to navigate to where snscrape36 is using the `cd` command ('cd' stands for 'change directory'). For example:
   - If you copied the `snscrape36` folder to Download, in the Command Prompt, type in:  
   `cd \Users\<your username>\Downloads\snscrape36`
   - If you copied into `Program Files`: `cd \PROGRA~1\snscrape36` 
     + `PROGRA~1` is shorthand for the "Program Files" folder
   - If you copied onto your Desktop, you should do:  
   `cd \Users\<your username>\Desktop\snscrape36`
3. Now, you can run the program from the Command-Prompt.
4. Let's say I want to get just the date and tweet contents of tweets with #AmericaFirst
   - Type in:  
   `snscrape36.exe --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst" > output.csv`
   - This will get my the 100 most recent results.
   - ***You can copy-paste any of the examples here and edit them in the Command Prompt.***
   - The output will be in the `output.csv` file; you can name this however you want.
   - The `.exe` part of `snscrape36.exe` is usually superfluous and can be left out, but we'll leave it in just for good style.
   - The `>` does something called 'redirection'. It takes the output of the program and sends it into the file `output.csv`.
   - The rest of the command are parameters/arguments to `snscrape36`.
5. Let's say I want 100 tweets occurring between May 1st and June 1st, 2018, type in (in one line):  
`snscrape36.exe --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > output.csv`
   * Refer to the Twitter search operators from slides #31-#33 in the Week 1 Hands-On for more info on the `since:` and `until:`.
   * Note that the scrape starts from the latest specified date and goes backwards in time until the number specified by `--max-results` is reached.
   * Because #americafirst is tweeted a lot, the 1st 100 tweets all occur on May 31, 2018.
5. Because the snscrape36 folder has a lot of other auxiliary files, you may want to save you output in the parent folder.
   * For this you could write `..\output.csv` in place of `output.csv`.
   * For example:  
`snscrape36.exe --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > ..\output.csv`
5. Here is an example that gets me more metadata, if I want to analyze those in Tableau:  
`snscrape36.exe --sleep 0 --max-results 100 --format {date},{username},\"{user.location}\",{user.followersCount},{user.friendsCount},{user.statusesCount},{user.favouritesCount},{user.verified},{lang},{source},{replyCount},{retweetCount},{likeCount},{quoteCount},\"{content}\",{url} twitter-search "#americafirst since:2018-05-28 until:2018-06-01" > output.csv`
6. If you want to analyze the tweets' text in SentiStrength, you'll need to use a tab rather than a comma as the delimiter:  
`snscrape36.exe --max-results 100 --format {date}\\t\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > output.txt`
   - Notice instead of a comma (,) separate each field, there's this weird `\\t`; this is that code for tab.
   - Also, notice we're outputting to a `.txt` file.
7. If you're requesting a lot of tweets, say more than 200, I suggest using a higher number of seconds for the `--sleep` option, to slow down the scrape.
   - Online services like Twitter (and other social media) don't like it when people scrape too fast.
   - I suggest a sleep setting of .2 seconds. This will make the scrape randomly delay .1 to .4 seconds per tweet. The process will then take about 26 seconds per 100 tweets.

### <a name="snscrape_mac"></a>SNScrape for Mac
1. [Click here](https://bit.ly/2ZIk2nT) to download the tool (a ZIP file)
   - Copy the top-level `snscrape36` folder out of the ZIP, e.g., Downloads or Desktop or wherever, just remember where you put it.
   - The Mac version has only been tested with Catalina and Big Sur.
   - I'll test it with slightly older versions soon.
1. Open the Terminal app
2. Now you need to navigate to where snscrape36 is using the `cd` command ('cd' stands for 'change directory'). For example:
   - If you copied the `snscrape36` folder to Downloads, in the Terminal, type in:  
   `cd ~/<your username>/Downloads/snscrape36` .
   - If you copied onto your Desktop, you should do:  
   `cd ~/<your username>/Desktop/snscrape36` .
3. Now, you can run the program from the Terminal
4. Let's say I want to get just the date and tweet contents of tweets with #AmericaFirst
   - Type in:  
   `./snscrape36 --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst" > output.csv`
   - This will get my the 100 most recent results.
   - ***You can copy-paste any of the examples here and edit them in the Terminal.***
   - The output will be in the `output.csv` file; you can name this however you want.
   - The `./` part of `./snscrape36` is needed to tell your Mac that `snscrape36` is in the current directory/folder.
   - The `>` does something called 'redirection'. It takes the output of the program and sends it into the file `output.csv`.
   - The rest of the command are parameters/arguments to `snscrape36`.
5. Let's say I want 100 tweets occurring between May 1st and June 1st, 2018, type in (in one line):  
`./snscrape36 --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > output.csv`
   * Refer to the Twitter search operators from slides #31-#33 in the Week 1 Hands-On for more info on the `since:` and `until:`.
   * Note that the scrape starts from the latest specified date and goes backwards in time until the number specified by `--max-results` is reached.
   * Because #americafirst is tweeted a lot, the 1st 100 tweets all occur on May 31, 2018.
5. Because the snscrape36 folder has a lot of other auxiliary files, you may want to save you output in the parent folder.
   * For this you could write `../output.csv` in place of `output.csv`.
   * For example:  
`./snscrape36 --sleep 0 --max-results 100 --format {date},\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > ../output.csv`
5. Here is an example that gets me more metadata, if I want to analyze those in Tableau:  
`./snscrape36 --sleep 0 --max-results 100 --format {date},{username},\"{user.location}\",{user.followersCount},{user.friendsCount},{user.statusesCount},{user.favouritesCount},{user.verified},{lang},{source},{replyCount},{retweetCount},{likeCount},{quoteCount},\"{content}\",{url} twitter-search "#americafirst since:2018-05-28 until:2018-06-01" > output.csv`
6. If you want to analyze the tweets' text in SentiStrength, you'll need to use a tab rather than a comma as the delimiter:  
`./snscrape36 --sleep 0 --max-results 100 --format {date}\\t\"{content}\" twitter-search "#americafirst since:2018-05-01 until:2018-06-01" > output.txt`
   - Notice instead of a comma (,) separate each field, there's this weird `\\t`; this is that code for tab.
   - Also, notice we're outputting to a `.txt` file.
7. If you're requesting a lot of tweets, say more than 200, I suggest using a higher number of seconds for the `--sleep` option, to slow down the scrape.
   - Online services like Twitter (and other social media) don't like it when people scrape too fast.
   - I suggest a sleep setting of .2 seconds. This will make the scrape randomly delay .1 to .4 seconds per tweet. The process will then take about 26 seconds per 100 tweets scraped.

### <a name="snscrape_final"></a>SNScrape - Final notes

* When reading an SNScrape output `.csv` file into Tableau, you should make sure to set the Text Qualifier to double-quote.
  - See slide #29 of Week 1 hands-on for where this happens.
  - This should not be an issue if you used tab as the delimiter (and saved as a .txt file).
* Also, after reading the file into Tableau, if you plan on doing any over time charts, make sure to transform the `date` column into "Date and time"
  - Right-click on the 'date' in the Dimensions pane -> Change Data Type -> Date & Time.
  - I've tried to alter the original code so that this wouldn't be needed, but it's not trivial to do!
* You can make the search more refined if needed. See [#BetterSearching](https://canvas.eur.nl/courses/31315/pages/faq-frequently-asked-questions?module_item_id=564386#BetterSearching) in the DMA FAQ.
