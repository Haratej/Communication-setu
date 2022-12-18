# Communication-setu
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" media="screen and (max-width:530px)" href="phone.css">
</head>
<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    html{
        scroll-behavior: smooth;
    }
    /*navbar */
    .navbar{
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0,0,0.5);
        position: sticky;
        top: 0;
    }
    .navbar ul{
        display: flex;
        list-style: none;
        margin: 20px 0px;
    }
    .navbar ui li{
        font-family: century;
        font-size: 1.1rem;
        font-weight: bold;
        font-size: x-large;
    }
    .navbar ul li a{
        text-decoration:rgb(150, 15, 15);
        color:black;
        padding: 8px 25px;
        transition: all .5s ease;
    }
    .navbar ul li a:hover{
        background-color: rgb(255, 255, 255);
        color: black;
        box-shadow: 0 0 10px white;
    }

    /* Home section */
    #home{
        display: flex;
        flex-direction: column;
        background-color: none;
        height: 1000PX;
        justify-content:center;
        align-items:center;
        color:maroon;
        font-size: x-large;
    }
    #home::before{
        content: "";
        position: absolute;
        top: 0;
        right: 0;
        background:url('://res.clhttpsoudinary.com/dsd8yegd2/image/upload/v1648454033/WhatsApp_Image_2022-03-28_at_1.19.13_PM_afrusn.jpg') no-repeat center center/cover;
        height: 1000px;
        width: 100%;
        z-index: -1;
        opacity: .8;
    }
    .main{
        display: flex;
        flex-direction: column;
        border: 1px solid white;
        align-items: center;
        position: absolute;
        top: 30%;
        right: 10%;
    }
    .headings{
        font-family: century;
        font-size: 3rem;
        text-align:center;
        margin: 40px 0px;
    }
    .btn{
        padding: 10x 35px;
        background-color: transparent;
        border: 1px solid white;
        color:black;
        outline: none;
        transition: .6s ease;
    }
    .btn:hover{
        cursor: pointer;
        background-color: white;
        color: black;
        box-shadow: 0 0 5px white,0 0 10px white,0 0 15px white;
        font-weight: bold;
    }

    /*About Selection */
    about{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        padding: 20px;
        margin-bottom: 50px;
    }
    #pic{
        display: flex;
    }
    #pic img{
        width: 575px;
        height: 400px;
    }
    #intro{
        display: flex;
        flex-direction: column;
        text-align: justify;
        padding: 10px;}
    #intro h2{
        font-size: 2rem;
        margin-bottom: 20px;
    }

    /* Picture Section */
    #pictures{
        display: flex;
        flex-direction: column;
        background-color: rgba(0, 0, 0, 0.9);
        color: white;
        align-items: center;
        padding: 20px;

    }
    .gallery{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        box-sizing: border-box;
    }
    .gallery img{
        width: 200px;
        height: 240px;
        margin: 10px;
    }

    /* Skills Section */
    #skills{
        display: flex;
        flex-direction: column-reverse;
        padding: 20px;
        align-items: center;
    }
    .row{
        display: center;
    }
    .box{
        display: flex;
        flex-direction: column;
        width: 550px;
        height: 450px;
        border: 1px solid rgb(82, 3, 3);
        margin: 10px;
        align-items: left;
        text-align: justify;
        padding: 10px;
        border-radius: 15px;
        background: linear-gradient(to top, rgb(119, 13, 13) 50%, white 50%);
        background-size: 100% 200%;
        transition: all .8s;
    }
    .box:hover{
        background-position: left bottom;
        color: rgb(243, 243, 243);
        border: none;
        box-shadow: 0 0 20px rgb(3, 3, 3);
    }
    .box image{
        width: 80px;
        height: 80px;
        background-color: white;
        padding: 10px;
    }

    /* contact section */
    #contact{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        background-color:black;
        color: white;
    }
    .form{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        align-items: center;
        margin: 20px 0px;
    }
    .input{
        padding: 12px;
        margin: 15px;
        width: 30%;
        border:none;
        outline: none;
    }
    footer p {
        text-align: center;
    }
    
    .experience-area h1 {
        padding: 5%;
    }
    
    .site-footer
    {
        background-color:black;
        padding:45px 0 20px;
        font-size:16px;
        line-height:24px;
        color:#737373;
    }
    .site-footer hr
    {
        border-top-color:#bbb;
        opacity:0.5
    }
    .site-footer hr.small
    {
        margin:20px 0
    }
    .site-footer h6
    {
        color:#fff;
        font-size:16px;
        text-transform:uppercase;
        margin-top:5px;
        letter-spacing:2px
    }
    .site-footer a
    {
        color:#737373;
    }
    .site-footer a:hover
    {
        color:#3366cc;
        text-decoration:none;
    }
    .footer-links
    {
        padding-left:0;
        list-style:none
    }
    .footer-links li
    {
        display:block
    }
    .footer-links a
    {
        color:#737373
    }
    .footer-links a:active,.footer-links a:focus,.footer-links a:hover
    {
        color:#3366cc;
        text-decoration:none;
    }
    .footer-links.inline li
    {
        display:inline-block
    }
    .site-footer .social-icons
    {
        text-align:center
    }
    .site-footer .social-icons a
    {
        width:60px;
        height:52px;
        line-height:40px;
        border-radius:100%;
        background-color:#33353d
    }
    .copyright-text
    {
        margin:0
    }
    @media (max-width:991px)
    {
        .site-footer [class^=col-]
        {
        margin-bottom:30px
        }
    }
    @media (max-width:767px)
    {
        .site-footer
        {
        padding-bottom:0
        }
        .site-footer .copyright-text,.site-footer .social-icons
        {
        text-align:center
        }
    }
    .social-icons
    {
        padding-left:0;
        margin-bottom:0;
        list-style:none
    }
    .social-icons li
    {
        display:inline-block;
        margin-bottom:5px
    }
    .social-icons li.title
    {
        margin-right:15px;
        text-transform:uppercase;
        color:#96a2b2;
        font-weight:700;
        font-size:13px
    }
    .social-icons a{
        position:relative;
        background-color:#eceeef;
        color:#818a91;
        font-size:30px;
        display:inline-block;
        bottom: 20px;
        line-height:44px;
        width:30px;
        height:34px;
        text-align:center;
        margin-right:8px;
        border-radius:100%;
        -webkit-transition:all .2s linear;
        -o-transition:all .2s linear;
        transition:all .2s linear
    }
    .social-icons a:active,.social-icons a:focus,.social-icons a:hover
    {
        color:#fff;
        background-color:#29aafe
    }
    .social-icons.size-sm a
    {
        line-height:34px;
        height:24px;
        width:24px;
        font-size:12px
    }
    .social-icons a.facebook:hover
    {
        background-color:#3b5998
    }
    .social-icons a.twitter:hover
    {
        background-color:#00aced
    }
    .social-icons a.linkedin:hover
    {
        background-color:#007bb6
    }
    .social-icons a.dribbble:hover
    {
        background-color:#5a5758
    }
    @media (max-width:767px)
    {
        .social-icons li.title
        {
        display:block;
        margin-right:0;
        font-weight:600
        }
    }
</style>
<body>
    <nav class="navbar">
        <ul>
            <img src="https://res.cloudinary.com/du3iufefj/image/upload/c_scale,w_73/v1670317439/Communication%20setu/WhatsApp_Image_2022-12-06_at_13.50.50_iocmo8.jpg" alt="">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About </a></li>
            <li><a href="#pictures">Pictures</a></li>
            <li><a href="#Skills">Services</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>
        
    <section id="home">
            <div class="Main">
                 <h1 class="Headings">COMMUNICATION_SETU<br></h1>
                 <button class="btn">
                    connecting together
              </button>
             </div>
         </section> 

        <section id="about">
            <h1 class="headings">About Communication Setu</h1>
            <div id="pic">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/c_scale,w_300/v1670321731/Communication%20setu/download_weumcj.jpg" alt="">
                <div id="intro">
                    <h2>We</h2>
                    <P>Communication Setu is a public friendly website working to help others in way of Information they want and it guides everyone helps as a barrier for Translation etc...                 

                    </P>
                </div>
            </div>
        </section>

        <section id="pictures">
            <h1 class="headings">Gallery</h1>
            <div class="gallery">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1670318208/Communication%20setu/WhatsApp_Image_2022-12-06_at_14.09.11_xj24h1.jpg" alt="">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1670318210/Communication%20setu/3_vcidwt.jpg" alt="">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1670318209/Communication%20setu/5_wbdjg4.jpg" alt="">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1670318209/Communication%20setu/4_jz1xga.jpg" alt="">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1670318206/Communication%20setu/6_pnqyqm.jpg" alt="">
            </div>
        </section>

        <center><section id="Skills">
            <h1 class="headings">Services</h1>
            <div class="row">
                <div class="box">
                   <center><h1 class="headings">We Support you</h1></center> 
                   <div align="left">
                   <li >We share the links regarding the Information you want.</li>
                    <li>The Reply can be given in your own Language:)</li> 
                    <li>We also give support through Whatsapp , Instagram also. </li>
                    <li>You can get Transport Information. </li>
                    <li> You can also get information about Hotels,Restaurants etc.</li>
                    </div>
                </div>

        </section></center>

        <section id="contact">
            <center><h1 class="heading">Contact Us</h1></center>
            <form action=""class="form">
                <input type="text" name="name" class="input" placeholder="communicationsetu@gmail.in">
                

            </form>
        </section>

        <footer>
            <!-- Add icon library -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<!-- Add font awesome icons -->


            <p>Follow Us on:</p>
         <!-- Footer -->
  <section id="footer">
    <div class="footer container">
      <div class="brand">
        <h1><span></span><span></span></h1>
      </div>
      <h2></h2>
      <div class="social-icon">
        <div class="social-item">
          <a href="https://instagram.com/communication_setu?igshid=YzdkMWQ2MWU=" target="_blank"><img src="https://res.cloudinary.com/du3iufefj/image/upload/c_scale,w_180/v1670320029/Communication%20setu/qrjpg_ycxz7d.jpg" /></a>
        </div>
        <div class="social-item">
          <a href="https://chat.whatsapp.com/IQQcZwNDWmp8LIVdcoJo4U" target="_blank"><img src="https://res.cloudinary.com/du3iufefj/image/upload/c_scale,w_75/v1670319750/Communication%20setu/479px-WhatsApp.svg_hxtr0r.png" /></a>
        </div>
      </div>
      <p>Copyright © 2022 Communication Setu. All rights reserved</p>
    </div>
  </section>
  <!-- End Footer -->
</body>
</html>
