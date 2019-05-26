{\rtf1\ansi\ansicpg1251\deff0\nouicompat\deflang1049{\fonttbl{\f0\fnil\fcharset0 Calibri;}{\f1\fnil\fcharset204 Calibri;}}
{\*\generator Riched20 10.0.17134}\viewkind4\uc1 
\pard\sa200\sl276\slmult1\f0\fs22\lang1033 #### Introduction\par
Hello, today I would like to tell you\f1\lang1049  \f0\lang1033 about CSS grid and I will try to explain\f1\lang1049  \f0\lang1033 why we should use it, how we can start\f1\lang1049  \f0\lang1033 using CSS grid and I will try to tell\f1\lang1049  \f0\lang1033 about its main advantages. So as web applications become more and more\f1\lang1049  \f0\lang1033 complex, we need a more natural way to\f1\lang1049  \f0\lang1033 create advanced layouts and CSS grid is\f1\lang1049  \f0\lang1033 a very exciting solution. So its main\f1\lang1049  \f0\lang1033 idea is that we divide our web page into\f1\lang1049  \f0\lang1033 columns and rows and we allow elements\f1\lang1049  \f0\lang1033 on this web page to take several rows\f1\lang1049  \f0\lang1033 and several columns if we need it. If\f1\lang1049  \f0\lang1033 we talk about flexbox, it's mostly\f1\lang1049  \f0\lang1033 helpful in positioning items in a one\f1\lang1049  \f0\lang1033 dimensional layout, but if we need two\f1\lang1049  \f0\lang1033 dimensional layouts, then CSS grid is a perfect choice. It provides\f1\lang1049  \f0\lang1033 tools for aligning and moving elements\f1\lang1049  \f0\lang1033 across both columns and rows.\par
#### Slide 1\par
 So let's\f1\lang1049  \f0\lang1033 take a look at this example. We have a\f1\lang1049  \f0\lang1033 container with class grid and inside it\f1\lang1049  \f0\lang1033 we have nine blocks. If we want to\f1\lang1049  \f0\lang1033 start using CSS grid, we just need to\f1\lang1049  \f0\lang1033 write\f1\lang1049  \f0\lang1033 display grid. But by default grid\f1\lang1049  \f0\lang1033 container has only one column, so if we\f1\lang1049  \f0\lang1033 add new blocks they will be on the new\f1\lang1049  \f0\lang1033 line and each of them gonna have width equal to container's width. But\f1\lang1049  \f0\lang1033 if we plan to use CSS grid, of course\f1\lang1049  \f0\lang1033 it's not our choice. \par
#### Slide 2\par
Let's imagine\f1\lang1049  \f0\lang1033 that we would like to divide our\f1\lang1049  \f0\lang1033 container into three equal columns. So we\f1\lang1049  \f0\lang1033 can do it by writing grid template\f1\lang1049  \f0\lang1033 columns. Our container has with 600\f1\lang1049  \f0\lang1033 pixels so in this case we have to write 200 pixels three times. \par
#### Slide 3\par
We also could\f1\lang1049  \f0\lang1033 use percents but the best\f1\lang1049  \f0\lang1033 way is to use fr. CSS grid\f1\lang1049  \f0\lang1033 introduced a\f1\lang1049  \f0\lang1033 new relative sizing unit, it is called fr or\f1\lang1049  \f0\lang1033 fraction. When we use fr unit we can define the size of columns and rows as a\f1\lang1049  \f0\lang1033 fraction of grid's length and width. \par
#### Slide 4\par
So\f1\lang1049  \f0\lang1033 let's take a look at grid template rows.\f1\lang1049  \f0\lang1033 We use it if we want to define rows and in\f1\lang1049  \f0\lang1033 this example I decided to make the\f1\lang1049  \f0\lang1033 second row as the biggest one so that's\f1\lang1049  \f0\lang1033 why I wrote 2 fr but we also can choose any value we wish. For example two\f1\lang1049  \f0\lang1033 fr\f1\lang1049  \f0\lang1033 for the first row, one fr for the\f1\lang1049  \f0\lang1033 second row and let's say ten fr for the\f1\lang1049  \f0\lang1033 third one. It's up to us to decide what\f1\lang1049  \f0\lang1033 we want and what our project needs.\par
#### Slide 5\par
Also\f1\lang1049  \f0\lang1033 let's talk about this situation. Let's\f1\lang1049  \f0\lang1033 imagine that we plan to divide our\f1\lang1049  \f0\lang1033 container into, for example, 12 equal\f1\lang1049  \f0\lang1033 columns. So of course we can use the first one and we can write one fr,\f1\lang1049  \f0\lang1033 one fr and do it 12 times. We can also\f1\lang1049  \f0\lang1033 use let's say 60 pixels or we can use 10\f1\lang1049  \f0\lang1033 percents but it's not the best solution.\f1\lang1049  \f0\lang1033 And fortunately in CSS grid now we have\f1\lang1049  \f0\lang1033 repeat function. So it allows us to write\f1\lang1049  \f0\lang1033 it in a very short way. So when we open\f1\lang1049  \f0\lang1033 parenthesis we just have two parameters.\f1\lang1049  \f0\lang1033 The first one is how many times we plan to repeat and the second one is what we\f1\lang1049  \f0\lang1033 plan to repeat. So in this example we use\f1\lang1049  \f0\lang1033 one fr but we can also use pixels or we can\f1\lang1049  \f0\lang1033 use percents. And as you see it allows us\f1\lang1049  \f0\lang1033 to reduce a huge\f1\lang1049  \f0\lang1033 amount of repeating\f1\lang1049  \f0\lang1033 code and it's really cool I guess.\par
#### Slide 6\par
Also I have to mention grid gap. So in my previous examples there was no space between our items. So\f1\lang1049  \f0\lang1033 now we can use grid column gap and great\f1\lang1049  \f0\lang1033 row gap to add some space between the\f1\lang1049  \f0\lang1033 items.\par
#### Slide 7\par
Ok now let's take a look at this\f1\lang1049  \f0\lang1033 example. Right now I'm going to use only\f1\lang1049  \f0\lang1033 one block and also I would like to add\f1\lang1049  \f0\lang1033 more columns and I would like to add\f1\lang1049  \f0\lang1033 more rows. In this example I plan to use\f1\lang1049  \f0\lang1033 four\f1\lang1049  \f0\lang1033 columns and six rows. Right now our\f1\lang1049  \f0\lang1033 block takes only one column and takes\f1\lang1049  \f0\lang1033 only one row. So we can imagine that our\f1\lang1049  \f0\lang1033 container is divided into\f1\lang1049  \f0\lang1033 four columns and six rows. Let's say that\f1\lang1049  \f0\lang1033 we want to create header. So we need our\f1\lang1049  \f0\lang1033 block to take all four columns. \par
#### Slide 8\par
To do it\f1\lang1049  \f0\lang1033 we can just write grid column 1 / 5. It\f1\lang1049  \f0\lang1033 means that we want our\f1\lang1049  \f0\lang1033 item to start at the first column and we\f1\lang1049  \f0\lang1033 want our item to end before the fifth.\f1\lang1049  \f0\lang1033 So the second value we write means before\f1\lang1049  \f0\lang1033 which column we would like our item to\f1\lang1049  \f0\lang1033 end.\par
#### Slide 9\par
Ok let's take a look at this example\f1\lang1049  \f0\lang1033 and right now let's we want the second item\f1\lang1049  \f0\lang1033 to take three columns and for example\f1\lang1049  \f0\lang1033 two rows.\par
#### Slide 10\par
We can simply do it just by writing grid row 2 / 4. Now we can't use one\f1\lang1049  \f0\lang1033 as the first parameter for grid row\f1\lang1049  \f0\lang1033 because the first row is already taken by our first element. That's why we have\f1\lang1049  \f0\lang1033 to write 2\f1\lang1049  \f0\lang1033 as the starting value to and we want it\f1\lang1049  \f0\lang1033 to end before the fourth row. And the same\f1\lang1049  \f0\lang1033 thing with columns we want it to start\f1\lang1049  \f0\lang1033 at the first column and end before the\f1\lang1049  \f0\lang1033 fourth column. So right now it takes three\f1\lang1049  \f0\lang1033 columns and two rows.\par
#### Slide 11\par
Ok now let's take\f1\lang1049  \f0\lang1033 a look at our next item. So at this\f1\lang1049  \f0\lang1033 moment it takes also one column and one\f1\lang1049  \f0\lang1033 row. Let's say that we want it to take for\f1\lang1049  \f0\lang1033 example three rows. \par
#### SLide 12\par
We can simply do it if we just write grid row 2 / 5.\par
#### Slide 13\par
So\f1\lang1049  \f0\lang1033 let's take a look at all the other items. As you can see using CSS grid we can\f1\lang1049  \f0\lang1033 create very complex layouts and it\f1\lang1049  \f0\lang1033 doesn't take a lot of time and I guess\f1\lang1049  \f0\lang1033 it's really cool. So CSS grid allows us\f1\lang1049  \f0\lang1033 to create very complicated and complex\f1\lang1049  \f0\lang1033 layouts and it can be very very helpful\f1\lang1049  \f0\lang1033 so in my opinion it's really cool and I\f1\lang1049  \f0\lang1033 definitely plan to use it. So I guess\f1\lang1049  \f0\lang1033 that's all. Thanks for your time and\f1\lang1049  \f0\lang1033 goodbye\par
}
 