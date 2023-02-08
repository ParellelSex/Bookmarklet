# Roblox Bookmarklet's

# Clothing Stealer
1. create a new book mark

2. edit the new bookmark and replace the url with the code string below

    ```javascript
    javascript:(function(){fetch('https://assetdelivery.roblox.com/v1/asset?id='.concat(window.location.href.split('/')[4]), { headers: { 'Accept': 'application/json' }}) .then(response => response.text()) .then(text => window.open("https://www.roblox.com/catalog/".concat(text.split('?id=')[1].split("<")[0])))})();
    ```
3. go to a roblox shirt/pants link and click the bookmark

# Join server with lowest players
1. create a new book mark

2. edit the new bookmark and replace the url with the code string below

    ```javascript
    javascript:(function(){fetch('https://games.roblox.com/v1/games/'.concat(window.location.href.split('/')[4]).concat('/servers/Public?sortOrder=Asc&limit=100')).then(response => response.json()).then((response) => { alert("Joining server with ".concat(response["data"][0]["playing"]).concat(" player'[s].")) ;Roblox.GameLauncher.joinGameInstance(window.location.href.split('/')[4],response["data"][0]["id"]) })})();
    ```
3. go to a game and click the bookmark
