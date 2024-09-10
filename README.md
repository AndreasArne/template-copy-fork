# template-copy fork
Workflows är inte aktiverad från början. Måste gå in och klicka manuellt.

För att pulla template-copy:

- git remote add upstream git@github.com:Webprogrammering-Lab/template-copy.git
- git fetch upstream # denna pular också branches som finns i template-copy. Oklar om vi vill eller om vi kan göra något åt det.
- git rebase upstream/master | borde inte använda denna. Gör istället `git merge upstream/main main`. Då slipper vi merge conflict att fixa med rebase. Nu säger den bara att det blir fel och då kan vi säga till studenter att göra `git checkout` på filerna de har ändrat i.

Det var drygt att fixa när det blev merge conflict. Men förhoppningen är ju att de inte ska få merge conflict eftersom de inte ska ändra i filerna.
