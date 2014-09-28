simpleviewer
============

A simple viewer for text and images, in 1 line of php and lots of lines of js.
Or, put longer, a mobile-ready mini-app to simply display cards with text and an image fed from simple JSON files that simply exist on a specific folder, making it easyish to use and customize by people who believe "XML" is something a car engine has.

#How it works
Essencially, the app is a slideshow of cards templated from data in the `dados` folder, obtained from all the .json files inside. That JSON data is then rendered through an [handlebars](http://handlebarsjs.com/) template, then displayed on a flexbox with a simple Object.Observe()-powered pagination mechanism to allow for user interaction. Uses [velocity.js](http://julian.com/research/velocity/) for the animation itself. Also uses HTML5 boilerplate but apparently who doesn't these days.

The cards are positioned left to right as per their names in the folder.
The JSON files themselves use the following template:
```
{
  "titulo": "I am a card title!",
  "texto": "I am long winded text! Lines and lines and lines of text!",
  "img": "Path to this card's image, relative to the './dados/' folder" 
}
```

If you use this for anything, let me know!
