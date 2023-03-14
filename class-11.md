# Class 11 notes

These topics matter because they help with the styling of a webpage and giving our page/site a better UI.

## Video and Audio Content

1. Since the 2000s, videos and audio are posted online everywhere all the time. They are very easily accessible and can deliver a lot of information.
2. The src attribute for the ```<video>``` element just contains the file path of the video. The controls attribute is for controlling the videos. That way you can play/pause the videos, skip ahead, or mute them.
3. It's important to have fallback content inside the video element in just case the video doesn't play or display for whatever reason.
4. One time ```<video>``` and ```<audio>``` met each other and then they fell in love and got married, so they decided to get into business together and so now we can watch videos that include audio if we want.

## Guide to Grids

1. Grids have a two-dimensional layout model and flexbox has a one-dimensional layout model.
2. The grid container is the parent element that contains the grid. You put the ```display: grid``` declaration in the grid container rule set in CSS. The grid items are the children elements of the grid container. The grid lines are the horizontal and vertical lines that make up the structure of the grid.

## Responsive images

1. Images are responsive when they changed their size based on the width of the device they are being displayed on. This is important because devices come in different sizes so if we want our images to be viewed the same for everyone no matter what device they're using, we have to make our images responsive.
2. The srcset attribute is for putting a number of photos at different sizes for the browser to choose from based on what size the browser is being displayed at. The sizes attribute says what image size would be best to choose based on media conditions that we set. Ex: ```srcset="img-480.jpg 480w, img-600.jpg 600px" sizes="(max-width: 500px) 480px, 600px"```
3. The srcset attribute is more helpful than using CSS to make responsive images because in CSS if you use something like media queries it loads all the images even if you're only displaying one. With srcset the browser picks and choose which image to load. With JavaScript, you can't change the image before it loads on the page so if you tried to change the image size, it would load both images.
