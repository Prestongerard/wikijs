<!-- TITLE: Sed -->
<!-- SUBTITLE: A quick summary of Sed -->

# sed

sed

sed -i -e s/<thing to change>/<thing to change it to>/g -e s/<other thing to change>/<other thing to change it to>/2  <file to change>

-i is an insertion flag. Lets you insert the changes into the targeted file

s/ means substitution

/g tells set to make the change for all instances of the thing to change in the file

Adding -e before the things to change lets you chain multiple changes into one command

/2 or really /<number> means change the <number> instance of that thing in a line

Look, sed is like super complicated but also SUPER flexible. It should probably have its own L&L one of these days. You can do a heck of a lot with it and really just like read this long guide or the one put out by Linode.