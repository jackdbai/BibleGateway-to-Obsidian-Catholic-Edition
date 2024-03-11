# BibleGateway-to-Obsidian: Catholic Edition
## Fork
This script modifies [selfire1's BibleGateway-to-Obsidian](https://github.com/selfire1/BibleGateway-to-Obsidian) script to download the Douay-Rheims version with the correct number and order of books. This is intentional as the this is the most notable public domain English Catholic version available on BibleGateway.

This version also adds chapter links to each .md of the book's files. This probably breaks breadcrumbs so that's been commented out.

Otherwise, the script is the same. [selfire1](https://github.com/selfire1) did some great work, credit goes to him.

## Additional Note
This is also not the same as [mkudija's BibleGateway-to-Obsidian-Catholic](https://github.com/mkudija/BibleGateway-to-Obsidian-Catholic) to specifically limit downloads to public domain DRA.

---

*Adapted original README below:*

---

## ⚠️ Disclaimer
This is not affiliated to, or approved by, BibleGateway.com. In my understanding it fits into the [conditions of usage](https://support.biblegateway.com/hc/en-us/articles/360001398808-How-do-I-get-permission-to-use-or-reprint-Bible-content-from-Bible-Gateway-?), but I make no guarantee regarding the usage of the script, it is at your own discretion.

## About
This script adapts [jgclark's BibleGateway-to-Markdown](https://github.com/jgclark/BibleGateway-to-Markdown) script to export for use in [Obsidian](https://obsidian.md/). It accompanies a [Bible Study in Obsidian Kit](https://forum.obsidian.md/t/bible-study-in-obsidian-kit-including-the-bible-in-markdown/12503?u=selfire) that gets you hands-on with using Scripture in your personal notes.

What the script does is fetch the text from [Bible Gateway](https://www.biblegateway.com/) and save it as a formatted markdown file. Each chapter is saved as one file and navigation between files as well as a book-file is automatically created. All the chapter files of a book are saved in its numbered folder.

## Installation
Here are the tools we are going to use:
* Our command line (Terminal)
* On Windows you might need to [install perl](https://www.perl.org/get.html).

## Setting ruby up
### Updating
In order to run the scripts, we will need to install ruby. Ruby comes pre-installed on macOS, but if you run into issues [update to the latest version](https://stackify.com/install-ruby-on-your-mac-everything-you-need-to-get-going/).

### Downloading BibleGateway-to-Markdown.rb
Follow the instructions to download and set up [jgclark's BibleGateway-to-Markdown](https://github.com/jgclark/BibleGateway-to-Markdown).

## Usage
### 1. Install scripts
Place both scripts (`bg2md.rb` and `bg2obs.sh`) in the same directory, open your terminal application, and navigate to that directory with commands like the following:

* `pwd` Show your current directory
* `ls` List all contents in the current directory
* `cd` Enter a subdirectory (e.g., `cd Desktop`)
* `cd ..` Brings you 'up' one directory

### 2. Run the script
Once you have navigated to the directory containing both scripts, run `bash bg2obs.sh`. This will run the bash script.

`NOTE`: In this directory, a folder called `Scripture` with subfolders like `Genesis`, `Exodus` and so on will be created.

### 3. Format the text in a text editor

Some cross references are sometimes still included, run `\<crossref intro.*crossref\>` to delete.

**There you go!** Now, just move the "Scripture" folder into your Obsidian vault. You can use the provided `The Bible.md` file as an overview file.
