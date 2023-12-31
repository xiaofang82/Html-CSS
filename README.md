# Html-CSS

## This is my first team assignment in MITT.

### This project is a travel company website that built using HTML and CSS language. The team member is Zhixin, Xiaofang(me) and Tieyao.  

My instructor Andre has certain requirements for the overall layout and color scheme of the website. We researched a lot of websites which are modern and fashionable. At the beginning we wanted build a website for information technology company, but after our discussion and experimentation, we ultimately chose a travel company website that can give us more space to design.  
  
Firstly, we unanimously decided to use blue as the color scheme, which is in line with our positioning for the website design. Tourism is like flying freely in the sky like a bird, and swimming in the sea like a fish.We have chosen artistic fonts for the title in the header section of the website to enhance aesthetics. The super banner uses a full screen landscape image with bold and enlarged text to highlight the entire website theme. I really like this design.  
![Super Banner](https://raw.githubusercontent.com/xiaofang82/Html-CSS/main/assets/img/superbanner.png)    
Here is also a small technique used to make the image less bright and make the text look more comfortable.  
> .hero {  
>     position: relative;  
>     background:   
>         linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)),  
>         url('../img/hero.webp') center center / cover no-repeat;  
> }  
>   
> .hero::after {  
>     position: absolute;  
>     inset: 0 auto auto 0;  
>     content: '';  
>     width: 100%;  
>     height: 100%;  
>     background-color: rgb(0 0 0 / 0.4);  
>     z-index: -2;  
> }  

Responsive website design is the most practical technique I have learned in this course. Changing the website layout according to the size of the browser makes the overall appearance more comfortable and does not cause clutter due to different devices. I am glad to have successfully applied it in this project.  

> @media screen and (max-width: 768px) {  
>     main .pic img{  
>         width : 100%;  
>     }  
>     main .column{  
>         width: 100%;  
>     }  
>     main .column:nth-of-type(1) {  
>         box-shadow: 0px 0px 0px;  
>     }   
>       
> }  
> 
> @media screen and (max-width: 480px) {  
>     .aboutus_column {  
>         width: calc(50% - 10px);  
>     }  
>       
> }  


* Laptop  
 ![Laptop](https://raw.githubusercontent.com/xiaofang82/Html-CSS/main/assets/img/contact1.png)
* Cellphone  
 ![Cellphone](https://raw.githubusercontent.com/xiaofang82/Html-CSS/main/assets/img/contact2.png)

The above two images show the effects displayed on Laptop and mobile phones, including a map where the positioning is done using the pseudo attribute’::before’. After I finished, I found that the position of the positioning icon always changes every time I adjust the size of the browser, and it is not an absolute positioning. I used Google to search for the reasons and solutions that caused this problem, and finally solved it through multiple experiments. The solution is to change the use of pixel positioning for the top, right, left, and bottom positioning attributes to use percentage.

> .maps {  
>     position: relative;  
> }  
>   
> .maps::before {  
>     display:inline-block;  
> 	  position:absolute;  
>     top: 46%;  
>     left: 52%;  
>     width: 40px;  
>     height: 40px;  
>     content: "";  
>     background-image: url("../img/spot.png");  
>     background-size: 40px;  
> }  

The four images on the homepage demonstrate the use of grid layout and response.  

> .column {
>     flex: 1 0 auto;
>     width: calc(25% - 20px);
>     height: 370px;
>     background-color: #fff;
>     box-shadow: 1px 1px 2px rgb(0 0 0 / 0.1);
>     cursor: pointer;
>     transition: all 0.15s ease-in-out;
> }
> 
> .column:hover {
>     box-shadow: 3px 3px 5px rgb(0 0 0 / 0.1);
>     transform: scale(1.02);
> }
> 
> .pic-1 {
>     background-color: white;
>     background: url('../img/Africa.jpg') no-repeat center center / cover;
> 
>     height: 240px;
> }
> 
> .pic-2 {
>     background-color: white;
>     background: url('../img/Europe.jpg') no-repeat center center / cover;
>    height: 240px;
>}
>
>.pic-3 {
>    background-color: white;
>    background: url('../img/Asia.jpg') no-repeat center center / cover;
>    height: 240px;
>}
>
>.pic-4 {
>    background-color: white;
>    background: url('../img/America.jpg') no-repeat center center / cover;
>    height: 240px;
>}

> @media screen and (max-width: 768px) {  
>    .column {  
>        width: calc(50% - 10px);  
>    }  
>}  
>  
> @media screen and (max-width: 480px) {  
>    .column {  
>         width: 100%;  
>     }  
> }  
![Index](https://raw.githubusercontent.com/xiaofang82/Html-CSS/main/assets/img/index4.png)

#### I hope to have a better grasp of the details in the next website project, such as viewing changes in text size and adjusting link colors on different devices.
