   
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css"/> -->
    <title>My Portfolio Website</title>
    <link rel="stylesheet" href="d2.css" type="text/css"/>
    
</head>

<body>
    <header>
        <a href="#" class="logo">Divine</a>
        <nav>
            <a href="#" class="active">Home</a> &nbsp; &nbsp;
            <a href="#">Services</a> &nbsp; &nbsp;
            <a href="#">Skills</a> &nbsp; &nbsp;
            <a href="#">Education</a> &nbsp; &nbsp;
            <a href="#">Experience</a> &nbsp; &nbsp;
            <a href="#">Contact</a> &nbsp; &nbsp;
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="woman-8161029_1280.png"   alt="">
        </div>
        <div class="home-content">
            <h1>Hi it's <span>Divine</span></h1>
            <h3 class="typing-text">I'm a<span></span></h3>
            <p>I am a math student and developer. I have basic knowledge in web dev (html, css and Js). I have a cetificate in web development
                I am also a logical thinker. I am willing to learn new skills in web development and also improve my skills.
            </p><br>
            <!-- <div class="social-icons">
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-github"></i></a>
                <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
            </div> -->
            <a href="#" class="btn">Hire me</a>
        </div>
    </section>
   <style>
      *{
    margin:0;
    padding:0;
   box-sizing: border-box;
   text-decoration: none;
   outline: none;
   border: none;
   font-family:Arial, Helvetica, sans-serif;
}

html{
    font-size:62.5%;
}

body{
    width:100%;
    height:100vh;
    overflow-x:hidden;
    background-color: black;
    color: whitesmoke;
}

header{
    margin-top: 20px;
    position:fixed;
    top:0;
    left:0;
    width:100%;
    padding:1rem 9%;
    background-color: transparent;
    filter:drop-shadow(10px);
    display:flex;
    justify-content: space-between;
    align-items: center;
    z-index:100;

}
.logo{
    font-size:3rem;
    font-family:serif;
    color: goldenrod;
    font-weight:800;
    cursor:pointer;
    transition:0.5s ease;
}
.logo:hover{
    transform:scale(1.1);
}

nav a{
    font-size: 1.8rem;
    color:white;
    margin-left:4rem;
    font-weight:500;
    transition:0.3s ease;
    border-bottom: 3px solid transparent;
}
nav a:hover,
nav a.active{
color: goldenrod;
border-bottom: 3px solid goldenrod;
}

@media(max-width:995px){
    nav{
        position:absolute;
        display:none;
        top:0;
        right:0;
        width:40%;
        border-left: 3px solid goldenrod;
        border-bottom: 3px solid goldenrod;
        border-bottom-left-radius:2rem;
        padding:1rem solid;
        background-color: black;
        border-top:0.1rem solid black;

    }
    
    nav.active{
        display:block;
        font-size:2rem;
        margin:3rem 0;
    }
    nav a:hover,
    nav a.active{
        padding:1rem;
        border-radius:0.5rem;
        border-bottom:0.5rem solid goldenrod;

    }
}

section{
    min-height: 100vh;
    padding:5rem 9% 5rem;
}
.home{
    display:flex;
    justify-content:center;
    align-items:center;
    gap:8rem;
    background-color: black;
}

.home-content h1{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size:6rem;
  font-weight:700;
  line-height: 1.3;
}
.home-content p{
    font-size:2rem;
}

span{
    color:goldenrod;
}

.home-content h3{
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight:700;

}

.home-img{
    border-radius: 50%;
}

.home-img img{
    position:relative;
    width:32vw;
    border-radius:50%;
    box-shadow: 0 0 25px solid goldenrod;
    cursor:pointer;
    transition:0.2s linear;
}

.home-img img:hover{
    font-size:1.8rem;
    font-weight:500;

}

.btn{
display:inline-block;
padding:1rem 2.8rem;
background-color: black;
border-radius:4rem;
font-size:1.6rem;
color:goldenrod;
letter-spacing:0.3rem;
font-weight:600;
transition:0.3s ease;
cursor:pointer;
}

.btn:hover{
    transform:scale3d(1.03);
    background-color: goldenrod;
    box-shadow: 0 0 25px goldenrod;
}

.typing-texxt span{
    position:relative;

}

.typing-text span::before {
content: "Web Developer";
color: goldenrod;
animation:words 20s infinite

}

.typing-text span::after {
    content: "";
    background-color: black;
    position:absolute;
    width:calc(100% + 8px);
    height:5%;
    border-left:3px solid black;
    right:-8;
    animation:cursor 0.6s infinite;
 }
 
    @keyframes cursor{
        to{
            border-left: 3px solid goldenrod;
        }
    }
    @keyframes words{
        0%, 20%{
            content:"Freelancer";
        }
        21%, 40%{
            content:"Web developer";
        }
        41%, 60%{
            content:"Web designer";
        }
        61%, 80%{
            content:"Data Analyst"
        }
        81%, 100%{
            content:"Mathlete..."
        }
    }

    @media (max-width:1000px) {
        .home{
            gap:4rem;
        }
    }
    

    @media (max-width:995px) {
        .home{
            flex-direction:column;
            margin:5rem 4rem;
        }
        
    }

    .home .home-content h3{
        font-size:2.5rem;
    }

    .home-content h1{
        font-size:5rem;
    }
    
    .home-img img{
        width:70vh;
        margin-top:4rem;
    }
    

    @media (min-width: 320px ){
        .home-img img{
            width:80px;
            margin-top:2rem;
        }
         body{
            width:100%;
        }
    }
    @media screen and (max-width: 800px) {
        .left, .main, .right {
          width: 100%;  
        }
        body{
            width:100%;
        }}
       
 
   </style>
</body>

</html>
