# Animated-Profile-Card-UI-Design-using
Profile Card UI Design

------HTML------

<!DOCTYPE html>
<html lang="PT-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="Style.css">
</head>
<body>
    <link class="A" rel="stylesheet" href="www.google.com">
    <div class="card">
        <div class="imgBox">
            <img src="./Imagens/FotoPessoal.jpeg" alt="#">
        </div>
        <div class="content">
            <div class="details">
                <h2>João Messias<br><span>Programador / Editor Designer</span></h2>
                <div class="data">
                    <h3>4<br><span>Portifolios</span></h3>
                    <h3>20<br><span>Post</span></h3>
                    <h3>220<br><span>Seguidores</span></h3>
                </div>
                <div class="actionBtn">
                    <button>Curriculo</button>
                    <button>Chat</button>
                </div>
            </div>
        </div>
    </div>
</body>
</html>

------CSS------

@import url('https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900');
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
body
{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: linear-gradient(45deg, #fbda61, #ff5acd);
}
.card
{
    position: relative;
    width: 350px; 
    /*height: 190px;*/
    height: 190px;
    background: #fff;
    border-radius: 20px;
    box-shadow: 0 35px 80px rgba(0,0,0,0.15);
    transition: 0.5s;
}
.card:hover
{
    height: 450px
}
.imgBox
{
    position: absolute;
    left: 50%;
    top: -50px;
    transform: translateX(-50%);
    width: 150px;
    height: 150px;
    background:#fff;
    border-radius: 20px;
    box-shadow: 0 15px 50px rgba(0,0,0,0.35);
    overflow: hidden;
    transition: 0.5s;
}
.card:hover .imgBox
{
    width: 250px;
    height: 250px;
}
.imgBox img
{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.card .content
{
    position: absolute;
    width:100%;
    height:100%;
    display:flex;
    justify-content: center;
    align-items: flex-end;
    overflow: hidden
}
.card .content .details
{
    padding: 30px;
    text-align: center;
    width: 100%;
    transition: 0.5s;
    transform: translateY(150px);
}
.card:hover .content .details
{
    transform: translateY(0px);
}
.card .content .details h2
{
    font-size: 1.25em;
    font-weight: 600;
    color: #555;
    line-height: 1.2em;
}
.card .content .details h2 span
{
    font-size: 0.75em;
    font-weight: 500;
    opacity: 0.5;
}
.card .content .details .data
{
    display: flex;
    justify-content: space-between;
    margin: 20px 0;
}
.card .content .details .data h3 span
{
    font-size: 0.85em;
    font-weight: 400;
    opacity: 0.5;
}
.card .content .details .actionBtn
{
    display: flex;
    justify-content: space-between;
}
.card .content .details .actionBtn button
{
    padding: 10px 30px;
    border-radius: 5px;
    border: none;
    outline: none;
    font-size: 1em;
    font-weight: 500;
    background: #ff5f95;
    color: #fff;
    cursor: pointer;
}
.card .content .details .actionBtn button:nth-child(2)
{
    border: 1px solid #999;
    color: #999;
    background: #fff;
}

