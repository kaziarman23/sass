<!-- How to install Sass. -->

1.We have to download a extention called "Live Sass Compiler".

<!-- vs code er setting e giye Sass er formate.json file ar moddhe path "/dist/css" thik kora (personal choice).  -->


 2.index.html file dist folder a create kore css er link korte hove.<!-- example: (href ="./css/main.css") -->


3.SCSS name ekta folder create korte hove tar moddhe "main.scss"


4.Then we have to activate "watch-Scss" extaintion.
It will create  an output and complie


NOW your good to go.
Now if we provide any style into our "main.scss" it will automatecally complied to our "main.css" file. 

<!-- we should not modifie "main.css" file rather we should modifie "main.Scss" file -->


 <!-- .............................. -->





<!-- variables in scss  -->

~The syntex is,
    $heading-color: red; <!-- this is an example-->

~To use it we have to write,
    $heading-color; 

~In variables we can use lot's of property,
    $font:(
        "regular": 400,
        "medium": 500,
        "bold": 700
    );
~Now we can use it's one property or all property,
    font-weight: map-get($font, bold);


<!-- .............................. -->




<!-- Nesting in scss  -->

~In main.scss file we can do nesting like this,
    .main{
        width: 100vw;
        height: 50vh;

        h1{
            color: black;
            font-size: 20px;

                &:hover{
                color: white;
                }
        }
    }
<!-- & this is for catching the parent element.We use this for avoid writing the full name of the parent element -->

<!-- .............................. -->



<!-- Partials in scss  -->

~We can create diffirent file and stor things.like for variable we can use one sparate file.

1.we have to create file in the Scss folder and before name it we have to give a underscore "_".

2.Then we can stor what we want.

3.Then we have to import the file to our "main.Scss" file,
    @import "./JustTheFileName"

<!-- .............................. -->
