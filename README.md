// So this is much easy to use than the cords so vote up and I will be very happy. You can press the skreen on the right side an then you will see mor stars coming up
// the Positions of the firt two stars
// the xPositions and  yPositions for the program
var xPositions = [100, 100];
var yPositions = [200, 100];
// wht is makking everithing happen is this var drawStars = function() { then what to happen };
var drawStars = function() {
    // the background call
    background(9, 5, 59);
    imageMode(CENTER);
    for (var i = 0; i < yPositions.length; i++) {
        // the star image
        image(getImage("space/star"), xPositions[i], yPositions[i], 30, 30);
    }
};
// what is makking the stars to be here 
drawStars();
// what will happen is the mous is cliked 
mouseClicked = function () {
    // for the x Position of the stars
   xPositions.push(mouseX); 
   // for the y Position of the stars
    yPositions.push(mouseY); 
    // what makes the stars to be there 
    drawStars();
    // the end
};
