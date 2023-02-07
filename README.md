# Bookmarklet
Roblox clothing stealer
[test](javascript:(function(){fetch('https://assetdelivery.roblox.com/v1/asset?id=%27.concat(window.location.href.split(%27/%27)[4]), { headers: { %27Accept%27: %27application/json%27 }}) .then(response => response.text()) .then(text => window.open("https://www.roblox.com/catalog/".concat(text.split(%27?id=%27)[1].split("<")[0])))})();)
