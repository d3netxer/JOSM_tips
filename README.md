# JOSM_tips
my own JOSM tips. JSOM is the advanced editor for OpenStreetMap



You can edit the tags of a large number of memory. It can use up more memory than JOSM usually needs however. When I tried to change the tags on over 6000 ways, it gave me an error box requesting more memory.

you can try a command like this (in Windows command prompt) (http://forum.openstreetmap.org/viewtopic.php?pid=500544):
java -Xmx1024M -jar D:\Downloads\josm-tested.jar

How to revert a changeset:
https://help.openstreetmap.org/questions/731/how-can-i-revert-a-changeset

Often you want to select many types of features at once and change something, like add a tag. You must be aware that dragging a rectangular box can select nodes as well as ways, but often you just want the tags on the ways. After your initial selection, in the Selection window you can click on the Search button and enter the following value to select only the ways (http://forum.openstreetmap.org/viewtopic.php?id=17632):

selected type:way

To copy and past only tags on a Mac:
-select feature you want to copy tags from:  Command key (⌘) + c
-select feature you want to paste the tags to:  Command key (⌘) + Shift + v
