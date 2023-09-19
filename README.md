# RandomizingFlow
## Short Description
MS Power Flow proof of concept for randomnly selecting from an Excel table.
## Install
1. Requires Microsoft Power Automate & MS OneDrive
2. Use the IMPORT feature and import the entire .zip package.
3. Copy the included spreadsheet to the root directory of your OneDrive
4. When you run the flow, a random pick of 3 choices will show up in your MS Teams chat.
## Context
The project was originally written to run every day at 530am where I work to pick three "volunteers" daily.
There are many statistical papers that show that the Excel random function is "pseudo-random," so a truly randomization is not achievable. In addition, when my staff would pick volunteers "randomly" there was a strong bias interference, so I needed something that would remove human bias and rely on natural processes. Cloudflare uses lava lamps to create a natural phenonmenon used in randomization of encryption keys. That randomization is available through Random.Org, which allows http requests to select a set of random numbers via open licensing. 
## Customize
The flow works by selecting the designated table "Table 1" from the designated spreadsheet, 'TestFile.xlsx' in the designated location, the root directory of your OneDrive. It is preconfigured to return three randomnly selected cells from the first column of the Excel table. Note, the table itself must be configured as an Excel Table  (Insert | Table). As it is now, the results are returned immediately. 
Illustration of flow:
![image](https://github.com/TheDrRichard/RandomizingFlow/assets/145368745/90de153d-6826-42cd-95c4-2b68b2904ba7)

To customize this flow, open Power automate, select the flow, and click on EDIT. 
a. Consider changing the conditions under which it starts. I use the "Recurrence" trigger in practice, so you'd want to change the "Manually trigger a flow" block. 
The 

