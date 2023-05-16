0:04
- Next step, let's recap, the essential CSS concepts
0:07
and properties you need to be comfortable with.
0:10
So the first thing is just including CSS in an HTML file.
0:15
Technically, I guess this falls
0:17
under the HTML elements video.
0:20
Let's make a new style sheet,
0:22
so I'll just do it here.
0:24
I'll call it app.css,
0:26
and let's include the style sheet.
0:29
So in my HTML file,
0:31
I need to add a link tag and that usually goes in the head
0:35
and then we'll set the href to be app.css
0:38
or whatever the path is that corresponds
0:41
to where that file is.
0:42
And then we need to add properties.
0:45
Let's style some stuff.
0:46
So you need to absolutely need
0:48
to understand CSS specificity.
0:51
You don't have to know the ins and outs.
0:53
You don't need to be able to calculate a specificity values.
0:57
I do have a YouTube video on that.
0:58
If you're curious about
1:00
how it all works behind the scenes,
1:01
but you need to understand why specificity matters.
1:05
And as an example,
1:07
if we have conflicting selectors
1:09
or conflicting styles,
1:11
like we have here,
1:12
we've got a div with an h1 inside of it.
1:15
The h1 has an id and the h1 has a class.
1:19
We're making all h1s Crimson.
1:22
Anything with the class of class style is violet
1:26
and anything with the id,
1:28
there should only be one element with that id,
1:30
is dodgerblue.
1:32
So what color wins if I select this
1:37
and just paste it over here,
1:39
somewhere in my HTML,
1:40
let's just do it up top.
1:42
And then I copy these three styles.
1:45
What color will my h1 be?
1:52
All right, we get blue for that h1,
1:55
the very first stage one that has the id and the class,
1:59
this other h1 was just here before.
2:02
So it's blue because an id selector
2:05
is far more specific than a class selector
2:08
or just an element selector like we have here.
2:12
So we end up with a blue h1,
2:14
and then our second h1 does not have a class
2:17
that doesn't have an id.
2:18
So it ends up Crimson
2:21
as all h1s will
2:23
as long as they don't have this class or this id.
2:28
And what if I were to add a class to that id,
2:32
the same class,
2:33
class dash style,
2:35
which color will it be now?
2:38
Well, this is more specific than all h1s.
2:41
So we get that color, which is violet.
2:45
So that's mostly what you need to know.
2:47
The fact that element selectors is not very specific.
2:50
Class selectors are more specific than elements
2:53
and id selectors are more specific than class selectors.
2:57
If you want a little bonus here,
3:00
what if instead of saying all h1s,
3:04
what if I added this, h1s that were inside of the body?
3:10
And I said, background to be green.
3:14
How about all of drab?
3:17
Okay.
3:19
What color will this h1 or this h1 be,
3:23
or if I add a third one in.
3:26
Which color will that h1 be?
3:28
So this style will apply to all of them.
3:31
They all are h1s.
3:33
And this one is actually more specific than we have here.
3:36
It's double the number of selectors,
3:38
even though an element selector is not that specific.
3:42
Two of them is still more specific than one.
3:45
So that one last h1 we just added, it does not have a class.
3:49
It doesn't have an id that matches,
3:50
it ends up with the olivedrab color.
3:54
All right.
3:55
You should also know when to use a class selector versus
3:58
when to use an id.
3:59
And when to add them to your HTML,
4:02
what's the general idea behind them.
4:04
And along with that, what's wrong with this code here.
4:08
I'll give you a hint.
4:09
It's on the left side.
4:10
What's wrong with what we have right here.
4:13
Take a moment.
4:15
We have two of the exact same id on two different elements
4:20
and id should be used at most once on each document.
4:23
So you can have as many ids as you want.
4:25
You usually don't want to have a ton,
4:27
but if you have a lot of different elements
4:29
that you need to style very differently from each other,
4:32
you can use an id,
4:33
but you should never repeat an id on the same page.
4:36
So id style, id style.
4:39
That's not good.
4:40
You don't wanna do that.
4:41
If we are trying to create multiple elements
4:44
with similar styles,
4:46
that's where a class comes in.
4:48
So we could create a class for these h1s
4:50
and add some styles for that class in our CSS,
4:54
but we don't wanna have a duplicate id on a page.
4:58
Properties that you should be familiar with
5:00
include things like background, color,
5:02
and color, font, family, font size,
5:06
cursor, border, text decoration,
5:11
just some of the basic visual changes.
5:14
I guess that's almost,
5:15
that's pretty much everything we do in CSS
5:17
is a visual change.
5:18
But you should be familiar with these properties
5:20
and you should be comfortable using a property you've
5:23
never used before.
5:25
What I mean by that is not just assuming
5:26
how it works and assuming what the name is,
5:28
but Googling it,
5:30
looking at the docs.
5:31
And if I said, add a text shadow,
5:33
which is different than a box shadow.
5:35
And if you've never used a text shadow,
5:37
you should be able to go Google it,
5:39
find some resource.
5:40
I like MDN, Mozilla Developer Network
5:43
and learn how it works.
5:45
Pretty much all the CSS properties,
5:47
they follow the exact same pattern, key,
5:49
the property name, colon, some value.
5:52
You just follow the rules and figure out what type of value,
5:55
what format CSS is expecting.
5:58
So you should be comfortable with a whole bunch
6:00
of those properties.
6:01
I'm not gonna go over all of them in detail here,
6:04
but just as a quick example, if we select,
6:06
how about spans?
6:09
Give them a background, color of purple.
6:13
If you don't know this yet,
6:15
that's my favorite color far and away.
6:18
And if it's not yours,
6:19
I think you're in the wrong course.
6:21
So we've got background color,
6:23
color which is different, right?
6:24
That's the text color.
6:26
So there we go, all of our spans have a purple background
6:29
with white text, things like text decoration,
6:34
where we can do things like line-through.
6:38
And this will give us crossed off spans,
6:41
font size.
6:44
There's quite a few options for sizes in CSS,
6:47
the different units.
6:49
So we could do 30 pixels.
6:53
If we've got larger ones.
6:55
We should also be familiar with things like rems.
6:58
So if I do 3 rems,
7:03
We get larger text.
7:05
What is a REM?
7:06
What does it stand for?
7:08
That's honestly the least important part.
7:10
But what does it actually mean?
7:12
How is it calculated?
7:13
What is 1 rem versus 2, versus 5?
7:16
So those are some examples of things you should know,
7:18
changing the font family, of course,
7:22
font family,
7:25
and I don't have any fancy fonts included.
7:28
We'll just go with Helvetica.
7:30
H-E-L-V-E-T-I-C-A,
7:34
there we go.
7:35
The font did change.
7:36
And then we've got font weight,
7:37
which we could use to change the thickness
7:41
or thinness of our text.
7:43
We could also just make it bold,
7:44
which is a shortcut.
7:45
All right, so now we've got bolded text.
7:48
Yeah, there's a bunch of properties.
7:49
Obviously we don't have time to go for all of them,
7:51
but make sure not that you're an expert
7:54
in every property and have them memorized,
7:56
but that you're comfortable finding new properties
7:58
and incorporating them into your own style sheets.
8:01
And then there's all the properties that have
8:03
to do with spacing.
8:05
So the box model,
8:07
things like padding and margin with,
8:09
and height, the border,
8:12
that's a big one.
8:13
So what are the different units we can use
8:15
for width and height?
8:16
We've got pixels.
8:17
We could use percentages.
8:19
We've got margin, padding.
8:21
What will this do?
8:23
What's the difference between margin
8:24
and padding around an element?
8:27
So on all spans, if I say the margin
8:30
is 20 pixels.
8:33
Before I refresh, where will the spacing go?
8:37
If I'm doing margin,
8:39
is it on all sides?
8:40
And then within this element,
8:43
it's on the outside of this box,
8:44
is it on the inside of this box?
8:46
If I refresh,
8:47
you'll see that the margin was added
8:49
to the outside of the actual element.
8:53
So the elements boundary is where that purple box ends
8:56
and then space was added outside of it.
8:59
Padding, on the other hand,
9:01
if I do 40 pixels,
9:05
is the spacing between the boundary and the content.
9:09
So that's our padding there.
9:11
You should understand the difference.
9:12
You should also be able to use properties
9:15
to specifically set padding on one side.
9:18
So patting top, 20 pixels.
9:22
Now we only have padding on the top,
9:26
also border, of course.
9:29
So border, if I want a 2 pixel
9:32
solid teal border,
9:35
you should be familiar with setting borders.
9:38
That's not quite large enough.
9:39
Let's do eight pixels
9:43
Other than border,
9:44
you should also be familiar with border radius.
9:47
So this allows us to curve the edges of our border.
9:51
Let's try 10 pixels and see what that looks like.
9:54
There we go.
9:55
We've got some rounded corners there
9:57
and I think that's enough at this point.
9:59
I don't have time and I don't wanna bore you
10:01
to death going over every single possible property,
10:05
but you should have good understanding of margin
10:06
and padding in particular.
10:08
And you should be able to style the top, the right,
10:10
the bottom and the left margin
10:12
and padding separately, also shorthand properties.
10:16
So there are shorthand properties for margin,
10:18
padding and border.
10:20
What does this mean?
10:23
What will have 10 pixels?
10:24
Which side?
10:26
Where will the 12 pixel margin go?
10:27
The 10 pixel margin,
10:28
the 8 pixel margin versus doing it this way,
10:33
which side to get 20 pixels,
10:35
same thing for padding.
10:36
And then here's the border shorthand.
10:39
You should also know that even though a lot
10:41
of people use this shorthand property,
10:44
you can do border with as a separate property
10:48
and change that to be 20 pixels,
10:51
and it's gonna be extra thick.
10:53
So this is setting border width here,
10:55
but you can also manually set it,
10:57
I guess both are manual,
10:58
but you can individually set it just like you can
11:01
with border color and border style.
11:04
And then we have positioning.
11:06
You should be familiar,
11:07
not with the crazy into and out of laying websites out,
11:11
creating responsive layouts.
11:13
You don't need to worry about that.
11:14
You don't need to worry about Flexbox if about it,
11:16
or if you've heard about it,
11:17
the CSS grid system you don't need to care about for now,
11:21
but you should be comfortable with the position property
11:24
and the different values like static,
11:27
fixed, relative and absolute.
11:30
So I know that's kind of a lot for one video.
11:33
Feel free to take your time going through some of this.
11:36
We're not gonna jump right into CSS right away.
11:39
So you have time to catch up if you need it,
11:42
but make sure that you go through these slides
11:44
or the notes or watch this video
11:46
and that you're able to nod your head along
11:48
to everything that I talk about or show you.
11:51
So that's a recap of the CSS skills
11:53
that you need before you really go through this course.
11:56
(Upbeat music)