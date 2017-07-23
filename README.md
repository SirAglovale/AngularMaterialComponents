# Material Design pure SASS

## Background
I started this project because I disliked a lot of the angular bindings for Material Design as they often require you to use their own components. I thought I would attempt to write a pure SASS/CSS Material Framework.

Bearing in mind that I am a sole developer, the naming conventions of some of the classes are less than ideal, however if you wish to fork this project and change names of classes or add functionality feel free.

## Colo(u)rs
Colo(u)rs in Material Design are defined on the google Material design page as Red 500 or Blue 800 e.t.c. As such I have taken another open source material colo(u)rs CSS framework which the syntax is as follows for

```HTML
<!--For changing the text colour-->
<div class=".color-<COLOUR NAME>-<SHADE>">

</div>
<!--For changing the background colour-->
<div class=".bg-<COLOUR NAME>-<SHADE>">

</div>
<!--For changing the border colour-->
<div class=".border-<COLOUR NAME>-<SHADE>">

</div>
```

## Depth
One of the main features of material design is the depth of materials this can be denoted in this framework also, there are 12 levels of depth

1 = Far from the user

12 = Close to the user

```HTML
<div class="dp-1">
    This div is far away from the user
</div>
<div class="dp-12">
    This div is close to the user
</div>
```

## Titlebar
This framework does not include a navbar element as of yet, this may be coming soon depending on my programming requirements. So far we have a titlebar which can be used as such

```HTML
<!--Define that a titlebar is being used. You should probably add a foreground and background colour to this and also a depth-->
<div class="titlebar dp-2 bg-blue-800 color-light-text-primary">
    <!--Now we insert a container to allow for the titlebar to dynamically resize with the rest of the webpage.-->
    <div class="container">
        <!--We add an image to denote the brand, this can be ommitted however I advise that you put your company logo here-->
        <img src="https://yourdomain.com/logo.png">
        <!--We also add a title that describes what the page does-->
        <span>Page Title</span>
    </div>
</div>
```

## Containers
As with a lot of frameworks we need some sort of container, we use the flexbox that is provided by CSS3 and SASS, our containers are divided up into 12 as it is the most divisible number.

```HTML
<!--Create a container-->
<div class="container">
    <!--Create a card of width 1-->
    <div class="card w-1 dp-3">
        <!--Do other card stuff in here-->
    </div>
    <!--Create a card of width 4-->
    <div class="card w-4 dp-3">
        <!--Do other card stuff in here-->
    </div>
    <!--Create a card of width 7-->
    <div class="card w-7 dp-3">
        <!--Do other card stuff in here-->
    </div>
</div>
```