#### Introduction
Hello, today I would like to tell you about CSS grid and I will try to explain why we should use it, how we can start using CSS grid and I will try to tell about its main advantages. So as web applications become more and more complex, we need a more natural way to create advanced layouts and CSS grid is a very exciting solution. So its main idea is that we divide our web page into columns and rows and we allow elements on this web page to take several rows and several columns if we need it. If we talk about flexbox, it's mostly helpful in positioning items in a one dimensional layout, but if we need two dimensional layouts, then CSS grid is a perfect choice. It provides tools for aligning and moving elements across both columns and rows.
#### Slide 1
 So let's take a look at this example. We have a container with class grid and inside it we have nine blocks. If we want to start using CSS grid, we just need to write display grid. But by default grid container has only one column, so if we add new blocks they will be on the new line and each of them gonna have width equal to container's width. But if we plan to use CSS grid, of course it's not our choice. 
#### Slide 2
Let's imagine that we would like to divide our container into three equal columns. So we can do it by writing grid template columns. Our container has with 600 pixels so in this case we have to write 200 pixels three times. 
#### Slide 3
We also could use percents but the best way is to use fr. CSS grid introduced a new relative sizing unit, it is called fr or fraction. When we use fr unit we can define the size of columns and rows as a fraction of grid's length and width. 
#### Slide 4
So let's take a look at grid template rows. We use it if we want to define rows and in this example I decided to make the second row as the biggest one so that's why I wrote 2 fr but we also can choose any value we wish. For example two fr for the first row, one fr for the second row and let's say ten fr for the third one. It's up to us to decide what we want and what our project needs.
#### Slide 5
Also let's talk about this situation. Let's imagine that we plan to divide our container into, for example, 12 equal columns. So of course we can use the first one and we can write one fr, one fr and do it 12 times. We can also use let's say 60 pixels or we can use 10 percents but it's not the best solution. And fortunately in CSS grid now we have repeat function. So it allows us to write it in a very short way. So when we open parenthesis we just have two parameters. The first one is how many times we plan to repeat and the second one is what we plan to repeat. So in this example we use one fr but we can also use pixels or we can use percents. And as you see it allows us to reduce a huge amount of repeating code and it's really cool I guess.
#### Slide 6
Also I have to mention grid gap. So in my previous examples there was no space between our items. So now we can use grid column gap and great row gap to add some space between the items.
#### Slide 7
Ok now let's take a look at this example. Right now I'm going to use only one block and also I would like to add more columns and I would like to add more rows. In this example I plan to use four columns and six rows. Right now our block takes only one column and takes only one row. So we can imagine that our container is divided into four columns and six rows. Let's say that we want to create header. So we need our block to take all four columns. 
#### Slide 8
To do it we can just write grid column 1 / 5. It means that we want our item to start at the first column and we want our item to end before the fifth. So the second value we write means before which column we would like our item to end.
#### Slide 9
Ok let's take a look at this example and right now let's we want the second item to take three columns and for example two rows.
#### Slide 10
We can simply do it just by writing grid row 2 / 4. Now we can't use one as the first parameter for grid row because the first row is already taken by our first element. That's why we have to write 2 as the starting value to and we want it to end before the fourth row. And the same thing with columns we want it to start at the first column and end before the fourth column. So right now it takes three columns and two rows.
#### Slide 11
Ok now let's take a look at our next item. So at this moment it takes also one column and one row. Let's say that we want it to take for example three rows. 
#### SLide 12
We can simply do it if we just write grid row 2 / 5.
#### Slide 13
So let's take a look at all the other items. As you can see using CSS grid we can create very complex layouts and it doesn't take a lot of time and I guess it's really cool. So CSS grid allows us to create very complicated and complex layouts and it can be very very helpful so in my opinion it's really cool and I definitely plan to use it. So I guess that's all. Thanks for your time and goodbye
