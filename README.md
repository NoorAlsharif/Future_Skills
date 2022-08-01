# Future_Skills
_Day3: CSS: Task 2 for Ministry of Communication and Information Technology's Future Skills (مهارات ـ المستقبل#)_

The task was to recreate a webpage and try to imitade the **CSS** we were given a sample image:

<p align="center">
  <img src="https://user-images.githubusercontent.com/71409736/182144230-9291a7bc-44a7-43bd-84c5-0776a09b32ac.jpeg" />
  <br>
  <img src="https://user-images.githubusercontent.com/71409736/182144245-ad2aabf7-dd4f-4246-b075-f715c8bc08e8.jpeg" />
  <br>
  <img src="https://user-images.githubusercontent.com/71409736/182144257-49764c8e-d567-415e-a27a-8086d4592371.jpeg" />
</p>

Here are my steps to completing the task:
## 1. HTML
- first i started by sectioning the webpage into 3 main sections using `HTML<div></div>`:
  - the header
  - the content
  - footer
- the header would contain a logo and the tittle.
- the content will feature four cards that hold a tittle name with a paragraph.
- the footer will simply hold my name.
## 2.CSS
- The first step was looking for a similar font to add. I endedd up finding `almarai`
```CSS
        @font-face {
            font-family: bukra;
            src: url(Almarai-Regular.ttf);
        }
```
- Then i add the logo with a background image to the div instead of the a simple gray color
```CSS
        #logo{
            height: auto;
            padding: 10px;
            margin:auto;
            text-align: center;
            background-color: #D8D8D8;

            background-image: url("bg light.png");
            background-size: cover;
            background-repeat: no-repeat;
        }

        img{
            filter: drop-shadow(1px 2px 2px #222);
        }
```
- the tittle div had a moving background. To achive this, simply use a `.gif` image
```CSS
        #title{
            height: auto;
            padding:5px;
            margin:0;
            text-align: center;
            background-color: #001860;
            border-top: solid 17px #1BCB80;
            color: white;
            box-shadow: 0 20px 8px 0 rgba(0, 0, 0, 0.20);
            line-height: 7px;
            text-shadow: 2px 2px black;

            background-image: url("bg.gif");
            background-position: bottom;
            background-size: cover;
            background-repeat: no-repeat;
        }
```
![tittle](https://user-images.githubusercontent.com/71409736/182146353-ac918693-db8c-4877-85c4-6067f5601257.gif)
