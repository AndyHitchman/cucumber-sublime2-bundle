# cucumber-sublime2-bundle

A bundle for [Sublime Text 2](http://www.sublimetext.com/2) that provides syntax coloring, snippets and auto-completion for [Cucumber](http://cukes.info/) and its [Gherkin](https://github.com/cucumber/cucumber/wiki/Gherkin) language.

## Installation
### Sublime Text 2
#### Mac OSX
    cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages
    git clone git://github.com/drewda/cucumber-sublime2-bundle.git Cucumber
#### Linux
    cd ~/.config/sublime-text-2/Packages
    git clone git://github.com/drewda/cucumber-sublime2-bundle.git Cucumber
#### Windows
    cd Users/<user>/AppData/Roaming/Sublime\ Text\ 2/Packages/
    git clone git://github.com/drewda/cucumber-sublime2-bundle.git Cucumber

###Sublime Text 3
#### Mac OSX
    cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages
    git clone git://github.com/drewda/cucumber-sublime2-bundle.git Cucumber
#### Windows (bash shell)
    cd Users/<user>/AppData/Roaming/Sublime\ Text\ 3\Packages
    git clone git://github.com/drewda/cucumber-sublime2-bundle.git Cucumber

Restart Sublime Text

## Table Cleaner

Aligns and cleans the tables for a prettier output. Useful for programming languages like Cucumber or LaTex.

### Before

![Table Cleaner Before](https://dl.dropbox.com/u/8314245/TableCleanerBefore.png)

### After

![Table Cleaner After](https://dl.dropbox.com/u/8314245/TableCleanerAfter.png)

### Usage
Select the table you want to clean, and press *alt + ;* and the table gets cleaned instantly.

### Settings
These settings can be found in Base File.sublime-settings
- **table_cleaner_delimiters** - Delimiters between two cells of the table - default: **["|", "&", "\\\\"]**
- **table_cleaner_align_to_middle** - Align the text of each cell to middle (if set to false, the text will be alligned to left) - default: **false**
- **table_cleaner_delimiters_white_spaces** - The number of whitespaces between the text of a cell and the delimiters - default: **1**

##Gherkin Phrase Auto-complete

Makes Gherkin phrases in cucumber feature files available as auto completions in Sublime Text. Table data for a phrase is also inserted.

###Example:

    Scenario: Auto-complete phrases in feature files
        Given a sublime text editor instance open in a cucumber folder
        When the user presses '<Ctrl>-Space'
        Then the auto-completion will show all phrases for Given/When/Then statements in all feature files
        And the user can type letters from the phrases to quickly find and re-use the phrase

1. Press `<ctrl>-space` to show the auto-complete box.
2. Type a few characters from words that matches a phrase above. The auto complete will show matching phrases.
3. Press enter (or tab) to insert. 

###Limitations
1. Currently only works in Sublime Text 3 (uses new async API methods). If you want this for ST2, then raise with @AndyHitchman
2. You need to save a modified file to pick-up updates in that file
3. Changes to feature files made outside of the editor are not detected.


## Credits
Created by the Github user @sagework, who pulled his/her repo from https://github.com/sagework/cucumber-sublime2-bundle

The Table Cleaner plug-in has been kindly contributed by [@mishu91](https://github.com/mishu91). If you'd like just the plug-in, without the rest of this Cucumber bundle, see his repository at https://github.com/mishu91/Sublime-Text-2-Table-Cleaner

The Gherkin Phrase Auto-Complete plug-in was contributed by [@AndyHitchman](https://github/AndyHitchman). if you'd like to use the plug-in, without the rest of this Cucumber bundle, see this repository at https://github.com/AndyHitchman/sublime-gherkin-auto-complete

I host this project at https://github.com/drewda/cucumber-sublime2-bundle for those who use Sublime Package Control.
