# fsjsDOM-Assingment

# Dom Manipulation Assignment

1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)



### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)

### My Code

```
document.querySelectorAll("h2.crayons-subtitle-2")[1].innerHTML="MOHAMMAD ZEESHAN";
document.querySelectorAll(".color-base-70")[1].innerText="I am a Full Stack Web Devloper";
```
### My Output

![Sample One](./out1.png)

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']


### My Code

```
let items=document.querySelectorAll("span.as-imagegrid-item-title");
let span=document.querySelectorAll("span.as-imagegrid-item-title span");
span.forEach((el)=>el.remove());
let arr=[];
items.forEach((el)=>arr.push(el.innerText));
console.log(arr);
```

### My Output

(7) ['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']




3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

### My Code

```
let containerId = document.querySelector(".accordion-homepage");
let addTab = document.createElement("section"); 
let newContent = document.createTextNode("My New FAQ"); 
addTab.appendChild(newContent); 
containerId.appendChild(addTab); 
addTab.setAttribute("id","newsection");
let sectionById = document.getElementById("newsection");
sectionById.style.background = "#FFFFFF";
sectionById.style.padding = "16px 52px 16px 64px";
sectionById.style.fontFamily = "'Google Sans', 'Google Sans Text', Roboto, sans-serif";
sectionById.style.borderTop = "thin solid #a9acaa";
sectionById.style.fontSize = ".875rem";
sectionById.style.fontWeight ="500";
```

### My Output

![Output](./out3.png)

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

### My Code

```
let div = document.querySelector(".one-tel-number");
div.innerText = "+91 1234567890";
```

### My Output

![Output](./out4.png)

5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)

### My Code

```
let mainDiv = document.querySelectorAll(".mytabs .diwali-deals-product-sale-pro .diwali-deals-product-sale-btn");
mainDiv.forEach((e) => {
    if(e.getAttribute("href") == "//www.samsung.com/in/smartphones/galaxy-z-fold4/buy/?modelCode=SM-F936BZKD"){
     e.innerText = "Check Out";
    }
} );
```

### My Output

![Output](./out5.png)

6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)

### My Code

```
let search = document.querySelector(".searchinput___19uW0");

function mouseOver(){
    document.querySelector(".searchinput___19uW0").style.backgroundColor = "Red";
}

search.addEventListener("mouseover", mouseOver); 
```

### My Output

![Output](./out6.png)

7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

### My Code

```

```

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

### My Code

```
let selectAlternateLanguages = document.querySelectorAll("#SIvCob a");
for (i = 0; i < selectAlternateLanguages.length; i++) {
  if(i % 2 == 0) {
    selectAlternateLanguages[i].remove();
  }
}
console.log(selectAlternateLanguages);
```

### My Output

![Output](./out8.png)


9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

### My code 

```
let heading = document.querySelector(".display-heading-1");
heading.style.color = "#B1361E"
heading.style.fontFamily = "monospace";
```

### My Output

![Output](./out9.png)


10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

### My code

```

```

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

### My Code

```
let icon = document.querySelector(".icon-logo");
icon.style.backgroundImage = "url('https://learn.ineuron.ai/_next/image?url=%2Fimages%2Fineuron-logo.png&w=750&q=75')"
```

### My Output

![Output](./out11.png)



12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

### My Code

```
document.querySelector('.btn-primary').style.backgroundColor = "Blue";
```

### My output

![Output](./out12.png)


13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

### My Code

```
document.querySelector(".fl-heading-text").textContent = "JSBOOTCAMP";
```

### My Output

![Output](./out13.png)


14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

### My Code 

```
document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "90px";

```
### My Output

![Output](./out14.png)



15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)


### My Code

```
let nameChange = document.querySelector(".section-title_title__VEDfK");
nameChange.innerHTML = "Start with Scratch"
```

### My Output

![Output](./out16.png)

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)

### My Code

```
let changeTodate = document.querySelector(".btn-container");
changeTodate.innerHTML = Date();

```

### My Output

![Output](./out17.png)

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

### My Code

```
let changeColor = document.querySelector(".p-f03-footer-container");
changeColor.style.background = 'none';
changeColor.style.backgroundColor = 'Orange';
```

### My Output

![Output](./out18.png)

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

### My Code

```
let sourceExtract = document.querySelector(".logo");
sourceExtract.getAttribute("Src");
```

### My Output

![Output](./out19.png)


20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

### My Code

```
let descColorChange = document.querySelector(".product-card-content .wide .desc");
descColorChange.style.color = "Orange";
```

### My Output

![Output](./out20.png)

