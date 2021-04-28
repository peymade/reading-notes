# Reading 14

## What Google Learned From Its Quest to Build the Perfect Team

Work has become more team-focused, and over the last two decades collaborative work has increased by 50%

While it may seem that collaboration would slow things down and decrease productivity, for software engineers it increases it- because bugs are caught sooner and solutions are arrived at faster. 

Google collected data and attempted to find patterns in what makes up a good team. But there weren't factors about the individual team members that were consistent across all productive teams. 

They found that each group had distinct norms, even if they weren't explicitly stated by the group leaders. 

A few commonalities were seen between successful groups in further research:

- People spoke roughly the same amount as other group members. There was equality in air-time
- Teams who had people who had higher emotional intelligence and who were more responsive to social cues, did better on tasks

**Psychological Safety** is the safety felt in taking risks around other people. It is having trust in those around you, and feeling like you can be yourself. This is the measure that researchers found to be most important to building a good group dynamic. 

## [CSS Animations](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

**transform** is a CSS property. It is not supported by all browsers. 
- Transform can affect objects on the 2D or 3D plane. 
- `transform: rotate(20deg)` rotates something 20 degrees clockwise
- `transform: scale(.50)` makes something 1/2 the original size
- The X and Y values can also be affected- stretching some object.
  - `transform: scaleX(.5)`
  - `transform: scaleY(1.15)`
- To move something from its position without affecting the flow of the page, use translate
  - `transform: translateX(-20)`
  - `transform: translate(-40px, 30%)`
  - `transform: skewX(5deg)`
- The transform origin is the center of the element. You can change it.
- Perspective origin acts similarly, and is useful for making things seem like they have depth

**transition** is used to change something about the element when it is in a certian state. The states are `:hover :focus :active :target`. The transition properties are:

- `transition-property` what property is targeted
  - properties such as background and border-radius can be targeted. You can target multiple, and separate them with commas
- `transition-duration` how long the transition takes
  - Can be set in s(seconds) or ms(milliseconds)
- `transition-timing-function` the rate at which the change happens
  - Can be specified in linear, ease-in, ease-out, and ease-in-out
- `transition-delay` delay after action 
  - Specified in the same way as transition-duration

You can add @keyframes to transitions, add a play state to pause and resume, and write animations in shorthand. 

## [8 Transitions](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

- Fade In
  - set opacity to .5, then when hovered over, set opacity to 1
- Change Color
  - set hover background color to different color
- Grow and Shrink
  - Use the scale transform property to grow (1.5) or shrink (.75)
- Rotate
  - Use rotate transform property and affect it by degrees
- Square to Circle
  - On the hover, set the border radius to a lower percentage
- 3D Shadow
  - On the hover, add a box shadow and move the element slightly
- Swing
  - Build and animation to move the element left and right, then apply it
- Inset Border
  - Give div class border, and add a shadow on the hover over it



~~~JavaScript
// Prototype function to play each note and store in storage
Note.prototype.handleClick = function() {
  if (recording === true) {
    recordingArray.push(this.audioID);
    let recordedStorage = JSON.stringify(recordingArray);
    localStorage.setItem(`storedKeys`, recordedStorage);
  }
  let x = document.getElementById(this.audioID);
  x.load();
  x.play();

  this.currentButton.classList.add('active');
  x.addEventListener('mouseup', this.stopActive.bind);
  }

  
Note.prototype.stopActive = function() {
  this.currentButton.classList.remove('active');
}

// Create constructor function to hold the name of the note, the audio ID, the mp3 path, and the button name
function Note(name){
  this.name = name;
  this.audioID = name + 'Note';
  this.normalMP3 = 'notes/' + name + '.mp3';
  this.buttonName = 'button' + name;

  

  // Point to the button on the HTML 
  this.currentButton = document.getElementById(this.buttonName);
  this.currentButton.addEventListener('click', this.handleClick.bind(this));


  console.log(this);
  allNotes.push(this);
}

let allNotes = [];

new Note('A3');
new Note('AS3');
new Note('B3');
new Note('C3');
new Note('CS3');
new Note('D3');
new Note('DS3');
new Note('E3');
new Note('F3');
new Note('FS3');
new Note('G3');
new Note('GS3');
~~~


[Home](https://peymade.github.io/reading-notes/)