# Welcome to Jed Saylor 👾

![logo](https://user-images.githubusercontent.com/95023449/143539159-06175af4-7dca-419b-a613-eb3b5fbe2b8f.png)

All the code in these repos was created and explained by Jed Saylor in his course.

To find help please visit:

[📺  Instagram](https://www.instagram.com/jedsaylor/)

# Jed Saylor Art Engine 🔥

![banner](https://user-images.githubusercontent.com/95023449/143539398-718265a8-90a4-43c3-821b-c299f2e40831.png)

Create generative art by using the canvas api and node js. Before you use the generation engine, make sure you have node.js installed.

## Installation 🛠️

If you are cloning the project then run this first, otherwise you can download the source code on the release page and skip this step.

```sh
git clone https://github.com/HashLips/hashlips_art_engine.git
```

Go to the root of your folder and run this command if you have yarn installed.

```sh
yarn install
```

Alternatively you can run this command if you have node installed.

```sh
npm install
```

## Usage ℹ️

Create your different layers as folders in the 'layers' directory, and add all the layer assets in these directories. You can name the assets anything as long as it has a rarity weight attached in the file name like so: `example element#70.png`. You can optionally change the delimiter `#` to anything you would like to use in the variable `rarityDelimiter` in the `src/config.js` file.

Once you have all your layers, go into `src/config.js` and update the `layerConfigurations` objects `layersOrder` array to be your layer folders name in order of the back layer to the front layer.

_Example:_ If you were creating a portrait design, you might have a background, then a head, a mouth, eyes, eyewear, and then headwear, so your `layersOrder` would look something like this:

```js
