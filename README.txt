A fanmade epub conversion of the Homestuck Epilogues. The main reason I did this is because I have trouble reading prose in large quantities on a typical computer or phone display, so I wanted to have a way to read the Epilogues on my ereader. It contains two appendices, Hussie's "Bridges and Off-Ramps" essay[1] sent in to be read on Perfectly Generic Podcast Episode 52, and Kate Mitchell's Medium post of expanded content warnings[2].

How it was made
===============

The bulk of the work was done using the EpubPress extension[3] for Firefox. All chapters for the current section (originally I had made separate files for the Prologue, Meat, and Candy) were opened sequentially in a browser window, then the Tab ReTitle extension[4] was used to reduce the tedium in changing the <title> elements for each chapter (as the official online version just has "The Homestuck Epilogues" as the HTML title for each chapter) before creating epubs with EpubPress. The default EpubPress covers and TOC pages were removed, custom covers added (after being quickly whipped up in the GNU IMP), and metadata set. Editing was done in Sigil[5].

I ended up deciding to combine the epilogues into a single file. I ended up manually unzipping my existing epubs and dumping Meat and Candy's OEBPS/Text folders into the Prologue's, manually adding them to the manifest in content.opf. Zipped back up, loaded back into Sigil, then added everything in order (Prologue ==> Meat ==> Candy) to the spine.

Then I decided to add the appendices. The essay was easy, just added the wiki page for the episode that as of this writing only has the transcribed essay to my Wallabag list and exported it as an epub from there, copying the html source from there and removing the blockquote elements. I could have also simply copypasted from my browser into PageEdit[6] but was overcomplicating things in my thought process. The Medium post was trickier, as Medium's HTML output is a huge mess of classes for each line. I ended up using Firefox's reader view and copypasting into PageEdit for cleaner HTML.

Finally, I copied the CSS class styles for each character's text colors from the Homestuck.com stylesheet. On e-paper displays this should provide different grayscale shades for each character's text in the script-style dialogues, making it easier to tell who is talking. I can at least confirm this works on Kobo devices.

Links
===== 

[1]: https://perfectlygeneric.fandom.com/wiki/Episode_52:_Semiotics,_Bridges,_and_Off-Ramps#The_Homestuck_Epilogues:_Bridges_And_Off-Ramps
[2]: https://medium.com/@gnvkay/homestuck-epilogues-content-warnings-2a7596bd0ad2
[3]: https://epub.press/
[4]: https://github.com/Lazyuki/ReTitle
[5]: https://sigil-ebook.com/
[6]: https://github.com/Sigil-Ebook/PageEdit