# Loopstudios-Landing-Page-FM Solution


This is my fourth Frontend Metnor challege [Loopstudios-Landing-Page](https://www.frontendmentor.io/challenges/loopstudios-landing-page-N88J5Onjw).

![Screenshot](desktop-preview.jpg)

## Overview

* Mobile First approach :ballot_box_with_check:
* SCSS :ballot_box_with_check:
* CSS Grid :ballot_box_with_check:
* Pixel perfect :ballot_box_with_check:

## Features

In order to further reduce the use of mk, I used the calculation for font size on padding, which proved to be successful, but I had to further limit the width to which the padding will grow.

First, calcualation starts from the smallest measure :

        padding-top: calc( 96px + (160 - 96) * (100vw - 375px) / (1440 - 375) );
        padding-left: calc( 24px + (164 - 24) * (100vw - 375px) / (1440 - 375) );
        padding-right: calc( 24px + (165 - 24) * (100vw - 375px) / (1440 - 375) );
        
 This works very well for font-sizes but not here on some reason the calculation continues to work even after the maximum width where it should otherwise stop. So I have to insert   media query myself      
