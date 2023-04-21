# T-o-Lao
Đăng các code cần nhớ thông qua notion
*{
    box-sizing: border-box;
    margin:0;
    padding:0;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 14px;
    color:#000;
    display: flex;
    flex-direction: column;
}
:root {
    --container-width: 1150px;
    --container-left-width:750px;
    --container-right-width: 360px;
    --color-orange: #FAA21B;
    --color-gray: #646464;
}
body div {
    /* Định dạng này chỉ để test layout */
    border:1px solid black;
    margin:5px;
    padding:5px;
}
img {
    width:auto;
    height: auto;
}
a {
    text-decoration: none;
}
.clearfix {
    clear: both;
}

.container {
    display: flex;
    flex-direction: row;
    border-style: none;
}
.container-full {
    border-style: none;
    width: 100%;
    margin: 0;
}
.bg-orange {
    background-color: var(--color-orange);
}
.bg-black {
    background-color: black;
}

/* HEADER */
#header {    
    display: flex;
    flex-direction: row;
    border-style: none;
    margin: 0;
}
#logo {
    width: 70px;
    height: 70px;
    border-style: none;
}
#hashtag {
    display: flex;
    flex-direction: row;
    width: 90%;
    height: 60px;   
    border-style: none;
    margin: 0;
}
#hashtag ul {    
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    width: 100%;
}
#hashtag li {
    width: 100%;
    display: flex;
    flex-direction: row; 
    margin: 4px;
    font-size: 12px;
    text-align: left;
    border-radius: 0.6em;
    border-style: groove;
}
#hashtag span {
    color: var(--color-orange);
}

/* MENU */
#menu {
    width: 100%;
    border-style: none;
}
#menu > ul {
    display: flex;
    flex-direction: row;
    width: 100%;
    align-items: center;
    justify-content: center;
    border-radius: 0.63em;
    background-color: var(--color-orange);
    border-style: none;
}
#menu > ul > li {
    margin: 5px 20px 5px 20px;
}
#menu > ul > li:hover {
    background-color: #646464;
}
#menu a {
    color: white;
}

/* CONTENT LAYOUT */
.content-left {
    width: 70%;
    border-style: none;
}
.content-right {
    width: 30%;
    border-style: none;
}
.row {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    border-style: none;
    
}
.column-1, .column-2, .column-3 {
    width: 32%;
    height: auto;
    border-style: none;

}
.column-lan {
    width: 49%;
    height: auto;
    border-style: none;

}
.column-ngoc {
    width: 49%;
    height: auto;
    border-style: none;
}
.column-3 {
    width: 100%;
    height: auto;
    margin: 0;
}

/* FOOTER */
#footer {
    display: flex;
    flex-direction: column;
}

#footer img
{
    width: 100px;
    height: 100px;
}
/* ANOTHER STYLES */
.section-title {
    font-size: xx-large;
    color: var(--color-orange);
    text-shadow: #646464;
    scrollbar-darkshadow-color: #646464;
    text-align: center;
}
.content-right .row.row .column-12 {
    width: 100%;
    height: auto;
    margin: 0;

}
.content-right .row.row .column-1 {
    width: 60%;
    height: auto;
}
.content-left .row{
    align-items: flex-start;
    justify-content: flex-start;
}
#footer .column-1 {
    color: white;
}
#footer .column-3{
    color: white;
}
.row .column-2
{
    width: 70%;
}
.container .content-right .row.row
{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
}
.rieng .column-2{
    width: 100%;
    border-style: none;

}
.hang2 ,.hang3 {
    display: flex;
    flex-direction: row;
    border-style: none;

}
.hang2 .column-2 , .hang3 .column-2 {
    width: 60%;

}
.hang2 .column-1 , .hang3 .column-1 {
    width: 40%;
    height: auto;
    border-style: none;

}
.col ,.col2 {
    border-style: none;

}
div.text {
    border-style: none;
    font-weight: bold;
}
.rieng , .rieng .column-12{
    border-style: none;

}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- header of page -->
    <div  id="header" class="container">        
        <div id="logo">
            <img src="images/logo.png" alt="">
        </div>
        <div id="hashtag">
            <ul>
               <li><span>#</span>VNTM All Stars</li> 
               <li><span>#</span>TheFace</li>
               <li><span>#</span>gương mặt thân quen</li>
               <li><span>#</span>Asia's Next Top Model 2017</li>
            </ul>
        </div>
    </div>

    <!-- menu bar -->
    <div class="container-full bg-orange">
        <div  id="menu" class="container">
            <ul>
                <li><a href="#">Trang chủ</a></li>
                <li><a href="#">Sao 24h</a></li>
                <li><a href="#">Thời trang</a></li>
                <li><a href="#">Điện ảnh</a></li>
                <li><a href="#">Âm nhạc</a></li>
                <li><a href="#">Đời sống</a></li>
            </ul>
        </div>
    </div>

    <!-- content of page -->
    <div class="container">
        <!-- left  content of page -->
        <div class="content-left">
            <div class="row">
                <div class="column-lan">
                    <img src="images/LanKhue-533x300.jpg" alt="">
                    <div class="col">Lan Khuê mạnh mẽ bốc lửa ủng hộ tinh thần đội tuyển Việt Nam tại SEA Games 29</div>
                </div>
                <div class="column-ngoc">
                    <img src="images/LyNaTrang-533x300.jpg" alt="">
                    <div class="col">Ly Na Trang khoe nhan sắc mỏng manh tựa sương mai trong tà áo dài truyền thống</div>
                </div>
            </div>

            <div class="row">
                <div class="column-1">
                    <img src="images/Cover-LacTroi-338x190.jpg" alt="">
                    <div class="col2">Cô gái cover ca khúc lạc trôi gây ấn tượng về vẻ ngoài nhí nhảnh</div>
                </div>
                <div class="column-1">
                    <img src="images/ThuTrang-338x190.jpg" alt="">
                    <div class="col2">Thu Trang từ Hoa Hậu Hài đến Mẹ Mưa</div>
                </div>
                <div class="column-1">
                    <img src="images/Dinh-Phuoc-338x190.jpg" alt="">
                    <div class="col2">Á Quân thần tượng bolero Đình Phước tăng tốc khởi động nhiều dự án âm nhạc</div>
                </div>
            </div>

            <div class="row">
                <div class="column-1"><img src="images/NgocDuyen-265x149.jpg" alt=""></div>
                <div class="column-2">
                    <div class="text">Kể chuyện về tình giữa người và yêu,Ngọc Duyên đăng quan quán quân Kịch cùng Bolero mùa đầu tiên</div>
                    <p class="text">Sự cạnh tranh ngang tài ngang sức giữa các đạo diễn Ngọc Duyên và đạo diễn Vũ Trần, danh hiệu quán quân đã thuộc về nữ đạo diễn...</p>
                </div>
            </div>

            <div class="row">
                <div class="column-1"><img src="images/NgoThanhVan-265x149.jpg" alt=""></div>
                <div class="column-2">
                    <div class="text">Ngô Thanh Vân và Jun Phạm trong ngày đầu bấm máy quay phim mới</div>
                    <p class="text">Sáng ngày 15/8 , đoàn phim về quê ăn tết do Ngô Thanh Vân sản xuất đã chính thức khai máy. Như đã thông tin từ...</p>
                </div>
            </div>

            <div class="row">
                <div class="column-1"><img src="images/NamEm-265x149.jpg" alt=""></div>
                <div class="column-2">
                    <div class="text">Hoa Hậu Nam em khai trang nhà hàng mang tên chính mình</div>
                    <p class="text">Trong tuần này,Hoa Hậu Trái Đất Việt Nam 2016 Nam Em đã chính thức khai trang nhà hàng ẩm thực với tên gọi N.E...</p>
                </div>
            </div>
        </div>    

        <!-- right content of page -->
        <div class="content-right">
            <div class="row">
                <div class="column-3">
                    <img src="images/Gintama-Poster-696x1031.jpg" alt="">
                </div>
            </div>
            
            <h3 class="section-title">Tin mới nhất</h3>
            
            <div class="rieng">
                <div class="column-12"><img src="images/XuanTruong-338x190.jpg" alt=""></div>
                <div class="column-2">
                    <div class="text">Thẩm Mĩ Viện Xuân Trường khai trương chi nhánh số 6</div>
                    <p class="text">Với thông điệp trả lại những gì thời gian đã lấy đi và mang đến những gì thiên nhiên không ban tặng,ngày 13/8/2017,Thẩm...</p>
                </div>
            </div>

            <div class="hang3">
                <div class="column-1"><img src="images/BadBoy-100x56.jpg" alt=""></div>
                <div class="column-2">Badboy Hải Ngoại Andy Quách ra mắt MV gáng mác 18+</div>
            </div>

            <div class="hang2">
                <div class="column-1"><img src="images/LanKhue-100x56.jpg" alt=""></div>
                <div class="column-2">Lan Khuê mạnh mẽ,bốc lửa ủng hộ tinh thần đội tuyển Việt Nam tham dự SEA GAMES 29</div>
            </div>
            
        </div>
    </div>
    
    <!-- footer of page -->
    <div class="container-ful bg-black">
        <div id="footer" class="container">
            <div class="row">
                <div class="column-1"><img src="images/logo.png" alt=""></div>
                <div class="column-1">INFO</div>
                <div class="column-1">CONTACT</div>
            </div>
            <div class="row">
                <div class="column-3">COPYRIGHT</div>                
            </div>
        </div>
    </div>
    
</body>
</html>
