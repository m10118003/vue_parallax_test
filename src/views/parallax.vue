<template>
    <div id="frame">
        <div id="menu">
            <img id="logo" src="data:image/png;base64,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" alt="">
            <ul id="links">
                <li id="top">
                    <a href="#bg-full-1" style="text-decoration:none;">Chunck</a>
                </li>
                <li id="center">
                    <a href="#bg-1" style="text-decoration:none;">Loin</a>
                </li>
                <li id="tail">
                    <a href="#bg-2" style="text-decoration:none;">Round</a>
                </li>
            </ul>
        </div>
        <div id="bg-full-1">
            <h1>SCROLL DOWN</h1>
        </div>
        <div id="bg-description">
            <h2>PARALLAX DEMO</h2>
            <p>Parallax scrolling is a web site trend where the background content is moved at a different speed than
                the
                foreground content while scrolling. Nascetur per nec posuere turpis, lectus nec libero turpis nunc at,
                sed
                posuere mollis ullamcorper libero ante lectus, blandit pellentesque a, magna turpis est sapien duis
                blandit
                dignissim. Viverra interdum mi magna mi, morbi sociis. Condimentum dui ipsum consequat morbi, curabitur
                aliquam pede, nullam vitae eu placerat eget et vehicula. Varius quisque non molestie dolor, nunc nisl
                dapibus vestibulum at, sodales tincidunt mauris ullamcorper, dapibus pulvinar, in in neque risus odio.
                Accumsan fringilla vulputate at quibusdam sociis eleifend, aenean maecenas vulputate, non id vehicula
                lorem
                mattis, ratione interdum sociis ornare. Suscipit proin magna cras vel, non sit platea sit, maecenas ante
                augue etiam maecenas, porta porttitor placerat leo.
            </p>
        </div>

        <div id="bg-1">
            <h1>LESS HEIGHT</h1>
        </div>

        <div id="bg-text">
            Scroll up and down to really get the feeling of how Cute This Cat Is.
        </div>

        <div id="bg-2">
            <h1>SCROLL UP</h1>
        </div>

        <div id="bg-text">
            Scroll up and down to really get the feeling of how This Cat So Long.
        </div>

        <div id="bg-2">
            <h1>SCROLL DOWN</h1>
        </div>
    </div>
</template>
<style>
        * {
            font-family: 'Roboto', sans-serif;
        }
        html {
            scroll-behavior: smooth;
        }
        body {
            margin: 0;
            padding: 0;
        }
        #frame {
            height: auto;
            width: auto;
        }
        #menu {
            position: fixed;
            width: 100%;
            z-index: 1;
        }
        #menu>#logo {
            width: 75px;            
            position: absolute;            
            border-radius: 10px;            
        }
        /* #box {
            height: 3%;
            width: 3%;
            background-color: royalblue;
            float: right;
            z-index: 1;
            position: relative;
            top: 80%;
            right: 95%;
            padding: 10px 10px;
            border-radius: 10px;            
            -moz-border-radius: 10px;
            -webkit-border-radius: 10px;
            text-align: justify;
        } */
        #links {
            margin: 0;
            padding: 0;
            position: fixed;
            right: 50px;
            float: both;
            z-index: 1;
            font-size: large;
            letter-spacing: 1px;
            text-decoration: none;
            text-align: justify;
            text-align: center;
            vertical-align: middle;
        }
        #menu>#links>li {
            display: inline-block;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
        }	/* 
			如果 display: inline 該元素的寬高只會受到元素本身的內容影響，
			width 及 height 及 padding 無法改變其寬高。
			*/
        /* #top {
            height: 15%;
            width: 15%;
            background-color: violet;
            float: right;
            z-index: 1;
            position: relative;
            top: -44%;
            left: -44%;
            padding: 10px 10px;
            border-radius: 10px;            
            -moz-border-radius: 10px;
            -webkit-border-radius: 10px;
            text-align: justify;
        } */
        /* #center {
            height: 15%;
            width: 15%;
            background-color: tomato;
            float: right;
            z-index: 1;
            position: relative;
            top: 50%;
            left: 50%;
            padding: 10px 10px;
            border-radius: 10px;
        } */  
        /* #tail {
            height: 15%;
            width: 15%;
            background-color: teal;
            float: right;
            z-index: 1;
            position: relative;
            top: 50%;
            left: 50%;
            padding: 10px 10px;
            border-radius: 10px;
        } */
        #bg-full-1, #bg-full-2 {
            position: relative;
            width: 100%;
            height: 100vh;
            background-image: url("~@/assets/img/1.jpg");
            background-size: cover;
            background-position: center top;
            background-attachment: fixed;
        }        
        #bg-full-1>h1,
        #bg-full-2>h1 {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            padding: 15px;
            background-color: rgba(255, 255, 255, 0.8);
            letter-spacing: 8px;
        }
        /* #bg-full>h1 {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            padding: 15px;
            background-color: rgba(255, 255, 255, 0.8);
            letter-spacing: 8px;
        } */
        #bg-description {
            padding: 50px, 80px;
        }
        #bg-description>h2 {
            text-align: center;
            letter-spacing: 6px;
        }
        #bg-description>p {
            text-align: justify;
            letter-spacing: 1px;
            line-height: 24px;
        }
        #bg-1 {
            position: relative;
            height: 35vh;
            background-image: url("~@/assets/img/1.jpg");
            background-size: cover;
            background-position: center center;
            background-attachment: fixed;
        }
        #bg-1>h1, #bg-2>h1 {
			position: absolute;
			top: 50%;
			left: 50%;
			transform: translate(-50%, -50%);
			padding: 10px;
			background-color: rgba(0, 0, 0, 0.5);
			color: #eee;
			letter-spacing: 8px;
		}
        #bg-text {
            height: 15vh;
            background-color: #333;
            padding: 7.5vh 80px;
            color: white;
        }
        #bg-2 {
            position: relative;
            height: 35vh;
            background-image: url("~@/assets/img/1.jpg");
            background-size: cover;
            background-position: center bottom;
            background-attachment: fixed;
        }
</style>