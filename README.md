## Devori.JS

Devori.js is a small and lightweight javascript file to handle device and its orientation.

### Idea

App tends to change to mobile first whereas we could easily adapt responsiveness for any devices using `@media` query. I am a developer, and I am so lazy to find out which exactly is demension of each device. As it turns out, I want to work with class's name instead of `@media` queries.

For an example, with `@media` you can control styles for `iphone` as below

```css
@media only screen 
and (min-device-width : 375px) 
and (max-device-width : 812px)
and (-webkit-device-pixel-ratio : 3) { /* STYLES GO HERE */}
```

Nonetheless, I want to have something similar to ...

```css
.tablet.tablet-8.portrait { /* STYLES GO HERE */ }
.iphone.iphone-5.landscape { /* STYLES GO HERE */ }
.iphone.iphone-6.portrait { /* STYLES GO HERE */ }
```

### Why?

Some poeple might ask for the reason why I need to make things more complicated, just use the `@media` queries.

OK! Let's take a look over advantages and disadvantages of both solution

`@media`:
 - Advantages:
  + Easy to control any devices if you know exactly its dimension
  + ... and more, you name it
 - Disadvantages:
  + Need to maintain devices' dimensions
  + Hard to read without comments
 
 `devori.js`
 - Advantages:
  + Easy to read and understand
  + No need to maintain devices' dimensions
 - Disadvantages:
  + Lacking abilities to fully control devices

### Conclusion

Discussing topic "What is better?" is likely same as "Which to use? IP Address or Domain name" :)
