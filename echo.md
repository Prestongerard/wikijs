<!-- TITLE: Echo -->
<!-- SUBTITLE: A quick summary of Echo -->

# Use Echos to announce what you’re doing in script

SUPER useful in debugging so you know where the StackScript failed

Provides feedback so people looking at the Lish console know where the StackScript is and if it’s done
# Use Echos to populate files
echo “text” > path/to/file

This will replace the contents of the file with what you’ve put in the echo

echo “text” >> path/to/file

This will add the text to the bottom of the target file.

Add the -e flag to add the text on a new line
