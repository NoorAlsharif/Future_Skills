# Future_Skills
_Day3: CSS: Task 2 for <a href="https://futureskills.mcit.gov.sa/ar/group/10178" target="_blank">Ministry of Communication and Information Technology's Future Skills (مهارات ـ المستقبل#)</a>_

The task was to create a webpage and try to replicate the **CSS** we were given a sample image:

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
## 2. CSS
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

- Next was the card div 
```CSS
        #card{
            margin-top: 80px;
            margin-bottom: 50px;
            height: 100px;
            height: min-content;
            box-shadow: 1px 6px 6px 2px rgba(0, 0, 0, 0.14);
            background-color: white;
            border-bottom: solid 5px #1BCB80;
            padding: 15px;
        }
```
- Inside the card div, the name tittle div, featured an animation that would transform the width of the div on hover
```css
        #name{
            background-color: #365D7E;
            width: 300px;
            height: auto;
            padding: 1px 10px 1px 0;
            line-height: 4px;
            color: white;
            font-stretch:wider;
            border-right: solid 10px #1BCB80;
            border-top-left-radius: 36px;

            /* Animate title card */
            -webkit-transition: width 1s ease-in-out;
            -moz-transition: width 1s ease-in-out;
            -o-transition: width 1s ease-in-out;
            transition: width 1s ease-in-out;
        }

        #name:hover{
            width: 1000px;
        }
```

![card](https://user-images.githubusercontent.com/71409736/182146993-fe212f91-b14c-4a27-b5d7-144cee2642b7.gif)

- Likewise, the green button on hover transfored its scale to `scale(1.2)`
```css
        #btn{
            background-color: #1BCB80;
            color: white;
            font-family: "bukra";
            border: none;
            padding: 5px;
            width: 130px;
            cursor:pointer;

            /* Animating card*/
            -webkit-transition-property: transform;
            -webkit-transition-duration: 0.2s;
            
            transition-property: transform;
            transition-duration: 0.2s;
        }

        #btn:hover{
            transform: scale(1.2);
        }
```
## 3. Final Result
The final webpage can be viewed <a href="https://future-skills-day2-task-nooralsharif.netlify.app/" target="_blank">Here.</a>

[![Netlify Status](https://api.netlify.com/api/v1/badges/6aa85c6f-fa11-4421-934a-71cf51bf6d37/deploy-status)](https://app.netlify.com/sites/future-skills-day2-task-nooralsharif/deploys)

### Badges
	https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white
  https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white
	https://img.shields.io/badge/VSCode-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white
  https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white
