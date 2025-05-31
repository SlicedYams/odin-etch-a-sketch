# odin-etch-a-sketch

Pseudocode

-Generating 16 x 16 grid of square divs
-We start with a container div
-we can make this a flex container with a flex direction of column
-we can then fill this with row containers, adding the square divs to each row container
-make each square change color on hover using an event listener

for 16 iterations:
    select the container
    create an inner-row-container
    make this flex container
    for 16 iterations:
        create a square div
        append it to the inner container
    append the inner-row-container to the main container

-now make this into a function that can be passed an integer for number of squares for length and width

generateGrid(num):

    for num iterations:
        select the container
        create an inner-row-container
        make this flex container
        for num iterations:
            create a square div
            append it to the inner container
        append the inner-row-container to the main container

-add a click event to the configure button at the top that prompts the user 
 for a number that sets the number of squares on the width and height

button.addEventListener("click", (event) => {
    loop until the value is between 1 - 100;
    prompt("Enter an integer to set the number of squares on the width and height");
})
