<!DOCTYPE html>

<html>

<head>
	<title>Simple web Development Template</title>
  <link rel="stylesheet" type="text/css" href="style.css"">
</head>
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

body {
  font-family: Georgia, "Times New Roman", Times, serif;
  color: white;
  background-color: black;
}

.container {
  max-width: 90rem;
  margin: 2rem auto;
  padding: 0px 2rem;
}

.img-fluid {
  max-width: 100%;
}
.logo img {
  width: 70px;
  height: 70px;
  border-radius: 41px;
  outline: 4px solid red;
}
nav {
  display: flex;
  justify-content: space-between;
  padding: 1rem 3rem;
  align-items: center;
}

.items {
  display: flex;
  align-items: center;
  gap: 30px;
}

.items a:link {
  text-decoration: none;
  color: white;
  font-size: 1.5rem;
  font-weight: bold;
}

.items a:hover {
  color: red;
}

.active {
  color: red !important;
}

button {
  font-size: 2rem;
  padding: 0.6rem 1rem;
  font-weight: bold;
  color: white;
  background: linear-gradient(to right, #c31432, #892211);
  border-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
  cursor: pointer;
  border: none;
}

button:hover {
  background: white;
  outline: 1px solid red;
  color: red;
  border: none;
}

.row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  justify-content: center;
  align-items: center;
}

.info {
  display: flex;
  flex-direction: column;
}
.short-info {
  color: red;
  font-size: 1rem;
  margin-bottom: 0.9rem;
}

.hero-heading {
  font-size: 3rem;
  margin-bottom: 0.3rem;
}
.hero-sub-heading {
  font-size: 0.9rem;
  opacity: 0.7;
}

.users {
  display: flex;
  align-items: center;
  margin: 1rem 0px;
}
.user {
  width: 20px;
  height: 20px;
  border-radius: 50%;
  border: 2px solid red;
}
.learn-more {
  align-self: start;
  margin-top: 3rem;
}

/* media queries */

@media only screen and (max-width: 800px) {
  .items {
    display: none;
  }

  .row {
    grid-template-columns: 1fr;
  }
  .learn-more {
    align-self: start;
    margin: 1rem 0px;
  }
}


<body>
	<nav class="navbar background">
		<ul class="nav-list">
			<div class="logo">
				<img src= "logo.png">
			</div>
			<li><a href="#web">Web Technology</a></li>
			<li><a href="#program">C Programming</a></li>
			<li><a href="#course">Courses</a></li>
		</ul>

		<div class="rightNav">
			<input type="text" name="search" id="search">
			<button class="btn btn-sm">Search</button>
		</div>
	</nav>

	<section class="firstsection">
		<div class="box-main">
			<div class="firstHalf">
				<h1 class="text-big" id="web">Web Technology</h1>
				<p class="text-small">
					HTML stands for HyperText Markup Language.
					It is used to design web pages using a markup
					language. HTML is the combination of Hypertext
					and Markup language. Hypertext defines the
					link between the web pages. A markup language
					is used to define the text document within tag
					which defines the structure of web pages.
					HTML is a markup language that is used by the
					browser to manipulate text, images, and other
					content to display it in the required format.
				</p>


			</div>
		</div>
	</section>

	<section class="secondsection">
		<div class="box-main">
			<div class="firstHalf">
				<h1 class="text-big" id="program">
					C Programming
				</h1>
				<p class="text-small">
					C is a procedural programming language. It
					was initially developed by Dennis Ritchie
					as a system programming language to write
					operating system. The main features of C
					language include low-level access to memory,
					simple set of keywords, and clean style,
					these features make C language suitable for
					system programming like operating system or
					compiler development.
				</p>


			</div>
		</div>
	</section>

	<section class="section">
		<div class="paras">
			<h1 class="sectionTag text-big">Java</h1>

			<p class="sectionSubTag text-small">
				Java has been one of the most popular
				programming language for many years.
				Java is Object Oriented. However it is
				not considered as pure object oriented
				as it provides support for primitive
				data types (like int, char, etc) The
				Java codes are first compiled into byte
				code (machine independent code). Then
				the byte code is run on Java Virtual
				Machine (JVM) regardless of the
				underlying architecture.
			</p>


		</div>

		<div class="thumbnail">
			<img src= "img.png" alt="laptop image">
		</div>
	</section>

	<footer class="background">
		<p class="text-footer">
			Copyright ©-All rights are reserved
		</p>


	</footer>
</body>

</html>
