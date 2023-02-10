## Reating Star


<br/>

concat js file

    <script type="text/javascript" src="js/reating-star.js"></script>
    
or

    <script type="text/javascript" src="js/reating-star.min.js"></script>
    
    
### Example for pure js

    <!doctype html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport"
                  content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
            <meta http-equiv="X-UA-Compatible" content="ie=edge">
            <title>Document</title>
        </head>
        <body>
            <div class="star-bar" arm-star-data-percent="50"></div>
            <div class="star-bar" arm-star-data-percent="10"></div>
            <div class="star-bar" arm-star-data-percent="25"></div>
            <div class="star-bar" arm-star-data-percent="100"></div>
            <div class="star-bar" arm-star-data-percent="71"></div>
            <div class="star-bar" arm-star-data-percent="88"></div>
            <div class="star-bar" arm-star-data-percent="37"></div>
            <script src="./js/reating-star.js" type="text/javascript"></script>
            <script type="text/javascript">
                StarReating.run('.star-bar', {
                    width: 15,
                    count: 5,
                    strokeWidth: 1,
                    stroke: 'rgba(0,0,0,1)',
                    starColor: 'rgb(255,200,0)',
                    starEmptyColor: '#FFFFFF',
                    points: 5,
                    onclick: function(starIndex, index) {
                        console.log('clicked', starIndex, index)
                    }
                });
            </script>
        </body>
    </html>