# Roblox Bookmarklet's

# Clothing Stealer
1. create a new book mark

2. edit the new bookmark and replace the url with the code string below

    ```javascript
    javascript:(function(){fetch('https://assetdelivery.roblox.com/v1/asset?id='.concat(window.location.href.split('/')[4]), { headers: { 'Accept': 'application/json' }}) .then(response => response.text()) .then(text => window.open("https://www.roblox.com/catalog/".concat(text.split('?id=')[1].split("<")[0])))})();
    ```
3. go to a roblox shirt link and click the bookmark
