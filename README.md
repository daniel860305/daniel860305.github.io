<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device-width, initial-scale=1, maximum_scale=1" />
	<meta charset="utf-8"></meta>
	<title>Lovely Little World</title>
	<style type="text/css">
	.head{background-color:#66B3FF;color:white;font-weight:bold;font-size:40px;
		padding:10px;text-align:center;text-shadow:0.1em 0.1em 0.2em black;
	}
	.head:hover{
		transform: scale(1.05);
		transition: .5s;
	}
	.content{width:1200px;margin-left:auto;margin-right:auto;
		text-align:center;}
	.box{width:400px;margin:10px;padding:10px;background-color:white;box-shadow:0px 0px 10px black;
		display:inline-block;vertical-align:top;
	}
	.box:hover{
		transform: scale(1.01);
		transition: .5s
	}

	/* 先做一個固定的區塊，再把圖片透過 object-fit 的方法放進去並讓其與區塊一樣大。*/
	.image_box{
		box-shadow:0px 0px 10px black;
		width:300px;height:400px;background:#aaa;margin:10px;
		overflow:hidden;
		display:inline-block;
	}
	/* 透過 hover 去感應區塊後修改圖片大小，並加上 transition 設定變形的轉場。*/
	img{
		transition: .5s; /* 提供漸進式變化 */
	}
	/* 虛擬選擇器搭配階層式選擇器 */
	.image_box:hover img{
		transform: scale(1.2); /* 放大1.2倍 */
	}
	.cover-fit{
		width:100%;height:100%;
		object-fit:cover;
	}
	.title{
		text-align:center;text-decoration:underline;
		text-shadow:0.05em 0.05em 0.1em black;
	}
	.small_box{
		width:300px;background-color:#eeeeee;
		text-align:left;line-height:30px;
		display:inline-block;
	}

	.name{
		font-weight:bold;font-size:24px;
	}
	table{
		width:250px;
		margin-left:25px;margin-right:25px;
	}
	.left{
		text-align:left;
	}
	.right{
		text-align:right;
	}
	.small_box a{
		color:#0000ff;
	}
	.text{
		margin-left:25px;margin-right:25px;text-align:justify;
	}
	.keyword{
		font-weight:bold;color:red;
	}
	.gallery_box{
		width:500px;height:500px;background:#aaa;
		margin:10px;box-shadow:0px 0px 20px black;
		display:inline-block
	}
	.gallery_box:hover img{
		transform: scale(1.1); /* 放大1.2倍 */
		box-shadow:0px 0px 20px black;
	}
	.space{
		margin:10px;
	}
	@media screen and (max-width:600px){
		.head{width:100%;font-size:30px;}
		.content{width:100%;text-align:center;}
		.gallery_box{width:350px;height:350px;}
	}
	</style>
</head>
<body style="margin-top:0px;background-color:#eeeeee">
	<div class="head">Nicole Chao & Daniel Tu</div>
	<div class="content">
		<div class="box">
			<div class="name">Nicole Chao</div>
			<div class="image_box">
				<img class="cover-fit" src="Nicole_Chao.jpg";/>
			</div>
			<div class="small_box">
				<div class="title"><h3>Information</h3></div>
				<table>
					<tr>
						<td class="left"><b>Height</b></td>
						<td class="right">163 cm</td>
					</tr>
					<tr>
						<td class="left"><b>Weight</b></td>
						<td class="right">48 kg</td>
					</tr>
					<tr>
						<td class="left"><b>Age</b></td>
						<td class="right">24</td>
					</tr>
					<tr>
						<td class="left"><b>Birth</b></td>
						<td class="right">1997.06.12</td>
					</tr>
				</table>
			</div>
			<div class="small_box">
				<div class="title"><h3>Personal profile</h3></div>
				<div class="text">Highly organized and pretty skilled at problem solving in graduate school. Skills include <span class="keyword">data analysis, good teamwork
				and presentation</span>. Able to understand customer demand and find out <span class="keyword">win-win</span> solution
				between company and customer.
				</div>
			</div>
			<div class="small_box">
				<div class="title"><h3>Contact information</h3></div>
				<ul>
					<li><b><a href="https://www.facebook.com/profile.php?id=100002946073299">Facebook</a></b></li>
					<li><b><a href="https://www.instagram.com/chaowei_6/?hl=zh-tw">Instagram</a></b></li>
					<li><b><a href="mailto:axga0000@gmail.com">axga0000@gmail.com</a></b></li>
					<li><b>Cellphone:</b> 0975-248-780</li>
					<li><b>Write to me: </b><input type="text" size="10px" /> <button id="btn">Send</button></li>	
				</ul>
			</div>
		</div>
		<div class="box">
			<div class="name">Daniel Tu</div>
			<div class="image_box">
				<img class="cover-fit" src="Daniel_Tu.jpg";/>
			</div>
			<div class="small_box">
				<div class="title"><h3>Information</h3></div>
				<table>
					<tr>
						<td class="left"><b>Height</b></td>
						<td class="right">173 cm</td>
					</tr>
					<tr>
						<td class="left"><b>Weight</b></td>
						<td class="right">66 kg</td>
					</tr>
					<tr>
						<td class="left"><b>Age</b></td>
						<td class="right">24</td>
					</tr>
					<tr>
						<td class="left"><b>Birth</b></td>
						<td class="right">1997.03.05</td>
					</tr>
				</table>
			</div>
			<div class="small_box">
				<div class="title"><h3>Personal profile</h3></div>
				<div class="text"><span class="keyword">Professional Taiwan Kartrider league player</span> in 2014. highly skilled at racing games, rhythm games, sports and study. 
				Able to go to gym <span class="keyword">6</span> times a week to strengthen my body and create <span class="keyword">win-win</span> relationship between Nicole nad myself.
				</div>
			</div>
			<div class="small_box">
				<div class="title"><h3>Contact information</h3></div>
				<ul>
					<li><b><a href="https://www.facebook.com/profile.php?id=100000582214483">Facebook</a></b></li>
					<li><b><a href="https://www.instagram.com/orevo860305/?hl=zh-tw">Instagram</a></b></li>
					<li><b><a href="mailto:daniel860305@gmail.com">daniel860305@gmail.com</a></b></li>
					<li><b>Cellphone:</b> 0938-525-509</li>
					<li><b>Write to me: </b><input type="text" size="10px" /> <button id="btn">Send</button></li>
				</ul>
			</div>
		</div>
	</div>
	<div class="space" />
	<div class="head">Gallery</div>
	<div class="space" />
	<div class="content">	
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_1.jpg"/>
		</div>
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_2.jpg"/>
		</div>
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_3.jpg"/>
		</div>
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_4.jpg"/>
		</div>
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_5.jpg"/>
		</div>
		<div class="gallery_box">
			<img class="cover-fit" src="Lovely Little World_6.jpg"/>
		</div>
	</div>
</body>
</html>
