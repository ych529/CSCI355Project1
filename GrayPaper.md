## Home
1.      <div class="circle-container">
            <div class="circle">
                <button id="close">
                    <i class="fas fa-times"></i>
                </button>
                <button id="open">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </div>
###### For this portion of the code, we consulted the Expanding Cards project on Udemy, which generates two buttons that let users open and close the navigation bar.
2.           <ul>
                <li>All bentoes has daily soup, chopsticks, and special homemade side dishes.
                </li>
                <li>Change fresh garnishes and soups daily!
                </li>
                <li>You can eat it anytime because the container is microwavable.
                </li>
            </ul>
Use the unordered list to add some general description of our product
3.      <div class="panel active"style="background-image: url(https://tokyo-kitchen.icook.network/uploads/recipe/cover/228831/94c857124ce91c81.jpg);">
            <h3>Pork</h3>
        </div>
        <div class="panel"style="background-image: url(https://d3l76hx23vw40a.cloudfront.net/recipe/gy08-017.jpg);">
            <h3>Beef</h3>
        </div>
        <div class="panel" style="background-image: url(https://img9.doubanio.com/lpic/s10385177.jpg);">
            <h3>Chicken</h3>
        </div>
        <div class="panel" style="background-image: url(https://www.paesana.com/hubfs/Blog/Italian-Fried-Seafood---Fritto-Misto-de-Mare.jpg);">
            <h3>Seafood</h3>
        </div>
In this case, we referred the Expanding Cards project from udemy and chose 5 images of various bentos as the focal point of our home page.
4.      <nav>
            <ul>
                <li><a href="../Home/Home.html"> Home</a></li>
                <li><a href="../Bento/Bento.html"> Bento</a></li>
                <li><a href="../Contact/Contact.html"> Contact</a></li>
            </ul>
        </nav>
To provide mutual access between the three websites in this case, we are using the nav element.
5.      body {
            font-family: "Times New Roman", Arial, Helvetica, sans-serif;
            color: #222;
            overflow-x: hidden;
            margin: 0;
        }
Set margin to "0" and body's font-color. 
6.      nav a:hover {
            color: #FF7979;
            font-weight: bold;
        }
The color and font-weight that will change when we hover over them.
7.      .panel h3 {
            font-size: 24px;
            position: absolute;
            bottom: 20px;
            left: 20px;
            margin: 0;
            opacity: 0;
        }
In Expanding Cards, we modified the text size and location of the bento names. Furthermore, we made these names to be fully translucent so that only active cards display the name.
8.      .panel.active {
            flex: 4;
        }
Set flexible items' length to 4.
9.      .circle-container {
            position: fixed;
            top: -100px;
            left: -100px;
        }
This section of code is significant because we set the backdrop of the open and close icons in page one to a fixed place in the upper left corner so that it does not shift when the nav bar increases.
10.     open.addEventListener('click', () => container.classList.add('show-nav'))
        close.addEventListener('click', () => container.classList.remove('show-nav'))
It implements the response and CSS effects when we click the open and close icons.

## Bento
1.     <nav>
            <ul>
                <li><a href="../Home/Home.html">Home</a></li>
                <li><a href="../Bento/Bento.html"> Bento</a></li>
                <li><a href="../Contact/Contact.html"> Contact</a></li>
            </ul>
        </nav>
To provide mutual access between the three websites in this case, we are using the nav element.
2.      <div class="search">
            <input type="text" class="input" placeholder="Search...">
            <button class="btn">
                <i class="fas fa-search"></i>
            </button>
        </div>
Create a search bar to make it easier for people to find their favorite bentos.
3.      <img src="https://www.dongchibd.com/upload/image/20201229/1609222372238570.png" width="20%" alt="Sausage Combo">
Insert the image so people know what this looks like.
4.      <ul>
            <li>Call: You can call in to order, pay when you pick up or on the delivery.</li>
            <li>Email: You can email to order, pay when you pick up or on the delivery.</li>
            <li>Walkin: You can walk in to our stores to buy and pay.</li>
        </ul>
Presented in an unsorted list, the content is easier to understand.
5.      <img src="https://www.dongchibd.com/upload/image/20201229/1609222244352519.png" width="20%" alt="Braised Beef Brisket Combo">
Fix the width of each image for cleaner typography.
6.      const search = document.querySelector('.search')
        const btn = document.querySelector('.btn')
        const input = document.querySelector('.input')
        btn.addEventListener('click', () => {
            search.classList.toggle('active')
            input.focus()
        })
This section of code can assist us in achieving hidden-search. If the customer knows exactly what they want. It will be a simple solution for them.
7.      <ol>
            <li>Crispy Chicken Thigh Combo</li>
            <li>Grilled Eel Combo</li>
            <li>Braised pork Combo</li>
            <li>Braised Beef Brisket Combo</li>
            <li>Cod fillet Combo</li>
        </ol>
Using the ordered list to show the ranking of bento selling.
8.      <p>
            <img src="https://static-resources.zybooks.com/star.png" alt="star">
            <img src="https://static-resources.zybooks.com/star.png" alt="star">
            <img src="https://static-resources.zybooks.com/star.png" alt="star">
            <img src="https://static-resources.zybooks.com/star.png" alt="star">
        </p>
Using image of stars to show how the bento is graded by customers to show how popular the bento is.
9.      <p>Cod is rich in protein, the meat is smooth and easy to digest, suitable for the elderly and children, and can help children and adolescents grow and develop. Cod is rich in DHA, DHA has the effect of promoting brain development, so eating cod often can make people smarter and protect eyesight. Cod is rich in magnesium and other minerals, which can prevent high blood pressure, myocardial infarction and other diseases, and can protect the cardiovascular system well. It also serves with 3 homemade side dishes, braised egg, braised tofu, and ham.</p>
We use the normal paragraph to show how the bento is made of and explain the advantage of the material that is good for human's health.

10.     <div>
            <h2>How do I pay for the order?</h2>
            <p>You have multiple payment methods. </p>
		    <ul>
			    <li>If your order is delivery order, your can pay cash, zelle, and paypal to the deliveryman. </li>
		    	<li>If your are picking up in store, you can using cash, card, zelle, and paypal in store when you are picking up.</li>
		    </ul>
        </div>
For each common question, we use one div to contain the question and also use list to display different answers under different conditions. 

## Contact
1.     <nav>
            <ul>
                <li><a href="../Home/Home.html">Home</a></li>
                <li><a href="../Bento/Bento.html"> Bento</a></li>
                <li><a href="../Contact/Contact.html"> Contact</a></li>
            </ul>
        </nav>
To provide mutual access between the three websites in this case, we are using the nav element.
2.             <table style="width:100%">
                <tr>
                    <th>Store Address</th>
                    <th>Phone</th>
                    <th>Email</th>
                </tr>
                <tr>
                    <td>1 HRT Ave, New York, NY 10001</td>
                    <td>917-777-0001</td>
                    <td>Feng.Hui1@Bento.com</td>
                </tr>
                <tr>
                    <td>2 Queens Blvd, Queens, NY 11367</td>
                    <td>917-777-0002</td>
                    <td>Feng.Hui2@Bento.com</td>
                </tr>
			  <tr>
                    <td>3 Bkly Ave, Brooklyn, NY 11678</td>
                    <td>917-777-0003</td>
                    <td>Feng.Hui3@Bento.com</td>
                </tr>
            </table>
We made a simple table including the name and location of our branch, as well as the name of our contact.
3.         <form id="info" method="post">
            <div class="formgroup" id="name-form">
                <label for="name">Your Name*</label>
                <input type="text" id="name" name="name" />
            </div>
            <div class="formgroup" id="email-form">
                <label for="email">Your E-mail*</label>
                <input type="email" id="email" name="email" />
            </div>
            <div class="formgroup" id="message-form">
                <label for="message">Your Message</label>
                <textarea id="message" name="message"></textarea>
            </div>
            <input type="submit" value="Send message!" /></div></form>
We construct a form allowing the user to enter their name and email address, as well as a textbox to fill up with relevant information.
4. @import url('https://fonts.googleapis.com/css?family=Muli&display=swap');
To import external fonts into CSS, we use the @import rule. We obtain the link to the desired font from "Google Fonts" and enter it in the url() function.
5. h1{
	font-weight: normal;
	font-size: 4em;
	margin:335px auto;
	width: 500px;
	color: #F90;
	text-align: center;
}
This section of code is pretty simple; it alters the font-size, font-weight, color, position, and other fundamental CSS characteristics of our page 3's h1 (aka "Contact us").
6. input:focus, textarea:focus{
	border: solid 3px #0F8FE8;	
}
The CSS code makes the border-width, border-style, and border-color values in input and texteara solid 3px #0F8FE8.
7. input[type="submit"]{
	background-color: #0F8FE8;
	color: white;
	height: 50px;
	cursor: pointer;
	margin-top: 30px;
	font-size: 1.29em;
}
input[type="submit"]:hover{
	background-color: #0FE83A;	
}
We change the background color of the submit button, the text size, and a few other fundamental CSS attributes here. We also provide the color change that occurs when the pointer passes over the button.
8. .bg {
    background: url('http://www.shanzhao119.com/style/images/about.jpg');
    position: absolute;
    top: -30px;
    left: -30px;
    width: calc(100vw + 60px);
    height: calc(100vh + 60px);
    z-index: -1;
    filter: blur(0px);
  }
We utilize a cafe image as the background when you enter the contact page.In order to limit the white space around the edges in the blurred state, we apply a calc when establishing the width and height values.
9. border: none;
	border-radius: 20px;
We set the border-radius to 20px to give the text box rounded corners and lessen overall sharpness.
10. function blurring() {
    load++
    if (load > 99) {
        clearInterval(int)
    }
    loadText.innerText = `${load}%`
    loadText.style.opacity = scale(load, 0, 100, 1, 0)
    bg.style.filter = `blur(${scale(load, 0, 100, 30, 0)}px)`
}
It implements the 0%-99% procedure and changes the entire page background from blurred to clear.
