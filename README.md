# FAIZ-TUITORIAL
PORT-FOLIO<br>
index.HTML <br>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My_Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
</head>
<body>
   <div class="wrapper">
        <div class="cover cover-left"></div>
        <div class="cover cover-right turn"></div>
        <div class="book">
            <div class="book-page page-left">
                <div class="profile-page">
                    <img src="img.JPEG" alt="">
                    <h1>Mohammad</h1>
                    <h3>fronterned engineer</h3>
                    <div class="social media">
                            <a href="#"><i class='bx bxl-linkedin' ></i></a>
                            <a href="#"><i class='bx bxl-facebook'></i></a>
                            <a href="#"><i class='bx bxl-whatsapp' ></i></a>
                    </div>
                            <p>Hi! I'm gland to see you, Lorem ipsum dolor sit, amet consectetur adipisicing elit. At dolores fuga doloribus eaque alias ullam assumenda, sint commodi exercitationem numquam magnam dolor nemo debitis, porro consequuntur aliquid culpa. Possimus, error!</p>
                        <div class="box-button">
                            <a href="/Resume.pdf" class="btn">Download CV</a>
                            <a href="#" class="btn
                            ">Contact Me</a>
                        </div>
                </div>         
            </div>
            <div class="book-page page-right turn" id="turn-1">
                <div class="page-front">
                    <h1 class="title">Work Experence</h1>
                
                    <div class="workedu-box">
                        <div class="workedu-containt">
                            <span class="year"><i class='bx bxs-calendar' ></i>2018 - 2019</span>
                            <h3>office executive</h3>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus tempore sit accusantium sint officia blanditiis impedit quas quos dolores doloremque.</p>
                        </div>
                        <div class="workedu-containt">
                            <span class="year"><i class='bx bxs-calendar' ></i>2020 - 2021</span>
                            <h3>office executive</h3>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus tempore sit accusantium sint officia blanditiis impedit quas quos dolores doloremque.</p>
                        </div>
                        <div class="workedu-containt">
                            <span class="year"><i class='bx bxs-calendar' ></i>2022 - 2023</span>
                            <h3>office executive</h3>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus tempore sit accusantium sint officia blanditiis impedit quas quos dolores doloremque.</p>
                        </div>
                        <div class="workedu-containt">
                            <span class="year"><i class='bx bxs-calendar' ></i>2023 - 2024</span>
                            <h3>office executive</h3>
                            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus tempore sit accusantium sint officia blanditiis impedit quas quos dolores doloremque.</p>
                        </div>
                    </div>
                    <span class="number-page">1</span>
                    <!-- next btn  -->
                    <span class="nextpre-btn" id="turn-1">
                        <i class='bx bx-chevron-right' ></i>                    </span>
                </div>


                <div class="book-page.page-left turn">
                    <h1 class="title">Education</h1>
                </div>
            </div>
        </div>
    </div>


<script src="script.js"></script>


</body>
</html>







<BR>
STYLE.CSS <BR>

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    font-family: "Poppins",sans-serif;
}
:root{
    --bg-color: #081b29;
    --main-color: #00abf0;
    --text-color: #333;
    --second-color: #555;
    --white-color: #fff;
    --cover-color: linear-gradient(45deg, #00abf0,#006e9a);
    --page-color: linear-gradient(90deg, #fff, #fff);
    --border: .125rem solid #00abf0;
    --box-shadow: 0 0 .6rem rgba(0,0,0, .2)
}

body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: var(--bg-color);

}

.wrapper{
    position: relative;
    width: 64rem;
    height: 45rem;
    padding: 2rem;
    box-shadow: 0 0 1.6rem rgba(0,0,0, .2) ;
    /* background-color: red; */
  

}

.cover {
    width: 50%;
    height: 100%;
    top: 0;
    left: 0;
    position: absolute;
    background:var(--cover-color);
    box-shadow: var(--box-shadow);
    border-top-left-radius: .6rem;
    border-bottom-left-radius: .6rem; 
    transform-origin: right;

}
.cover.cover-left{
    z-index: -1;
}

.cover.cover-right.turn{
    transform:rotateY(180deg);

}


.book{
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
}


.book .book-page{
    position: absolute;
    width: 50%;
    height: 100%;
    padding: 2rem;
    background: var(--page-color);
    box-shadow: 0 0 .6rem rgba(0,0,0, .1);
    display: flex;
    
}

.profile-page{
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}


.profile-page img{
    max-width: 190px;
    border-radius: 50%;
    border: .25rem solid var(--main-color);
    margin-bottom: .8rem;
}


.profile-page h1{
    font-size: 2.7rem;
    line-height: 1;
}

.profile-page h3{
    font-size: 1.5rem;
    color: var(--main-color);
}

.profile-page .social.media a{
    display: inline-flex;
    font-size: 1.5rem;
    width: 2.5rem;
    height: 2.5rem;
    border: var(--border);
    background: transparent;
    border-radius: 50%;
    align-items: center;
    justify-content: center;
    color: var(--main-color);
    margin: .5rem;
    transition: .5s;
}

.profile-page .social.media a:hover{
    background-color: var(--main-color);
    color: #fff;
}

.profile-page p{
    text-align: justify;
}

.profile-page .box-button{
    margin: 1.2rem;
}
#p {
    margin: 2rem;
}

.btn{
    display: inline-flex;
    font-size: 1.3rem;
    border: var(--border);
    color: var(--white-color);
    align-items: center;
    justify-content: center;
    width: 9.5rem;
    height: 3rem;
    border-radius: .3rem;
    margin: .8rem;
    background: transparent;
    transition: .5s;
    background: var(--main-color);
    transition: .5s;
}

.btn:hover{
    background: transparent;
    color: var(--main-color);
}

.box-button .btn:nth-child(2){
    color: var(--main-color);
    background: transparent;

}

.box-button .btn:nth-child(2):hover{
    background: var(--main-color);
    color: var(--white-color);
}

.book-page.page-right{
position: absolute;
right: 0;    
transform-style: preserve-3d;
}


.book-page .page-right.turn{
    transform: rotateY(-180deg);
}

.book-page .page-front,
.book-page .page-back{
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    background: var(--page-color);
    padding: 1.5rem 2rem;
}

.book-page .page-front{
    transform: rotateY(0deg) translateZ(1px);
}

.book-page .page.page-back{
    transform: rotateX(180deg) translateZ(1px);
}

.workedu-box{
    margin-top: 2.5rem;
    border-left: var(--border);

    
}


.workedu-box .workedu-containt{
    position: relative;
    padding-left: 1.6rem;
    margin-bottom: 1.2rem;
}

.workedu-box .workedu-containt::before{
    content: '' ;
    position: absolute;
    top: 0;
    left: -.55rem;
    width: 1rem;
    height: 1rem;
    background: var(--main-color);
    border-radius: 50%;
}


.title{
    text-align: center;
    margin-bottom: 1rem;
}

.year{
    color: var(--main-color);
}
.year i{
    margin-right: .4rem;
}

.number-page{
    position: absolute;
    bottom: 1.2rem;
    left: 50%;
    transform: translateX(-50%);
    justify-content: center;
}

.nextpre-btn{
    position: absolute;
    bottom: 0.9rem;
    right: 2rem;
    width: 2rem;
    height: 2rem;
    font-size: 2rem;
    display: inline-flex;
    justify-content: center;
    cursor: pointer;
    transition: .5s;
}

.nextpre-btn:hover{
    color: var(--main-color);
}


