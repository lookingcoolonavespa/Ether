The repository has moved to https://github.com/nksupermarket/Ether. 
The new tab page is now https://nksupermarket.github.io/Ether/.

To restore your old settings follow these steps: 

1) go to https://lookingcoolonavespa.github.io/Ether

2) open your developer tools by pressing `Ctrl + Shift + I` 

3) go to the `console` tab

4) copy and paste this code into the input 
```
const config = [
  "keybinds",
  "links",
  "theme",
  "image",
  "search",
  "custom search details",
].reduce((acc, curr) => {
  return { ...acc, [curr]: JSON.parse(localStorage.getItem(curr)) };
}, {});
JSON.stringify(config, null, 0);
```
5) copy everything inside the single quotes eg. 'copy everything inside here' <-- just the text 

6) go to https://nksupermarket.github.io/Ether and go to the settings

7) scroll down `import json`, paste everything there and save
