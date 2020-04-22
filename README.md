# Intro to Coding Portfolio Build
---

Start by welcoming and explaining why coding is important.  Explain why Eleven Fifty is a good place to learn how to code and how the tech industry allows for people to have a fast-paced learning environment for a short amount of time and how that could get them a good job in this career path.

OPTIONAL - have them break into small groups, draw a house on a whiteboard, and have them list step-by-step instructions of how to draw it.  This should demonstrate what it is like to think like a programmer.  Also helps them start to get to know each other.

---

### Setup
Have everyone create an account on CodePen and start a pen.

---

### HTML Basics

Explain that CodePen is a quick tool to build out a webpage, test animations, test `CSS` selectors, but not a tool for a fully deployed website. You might touch on how the boxes are already linked together, and that the Body tag is where the `HTML` goes.

Now go to your `CSS` box and add the following:

```css
body {
  background-color: lightblue;
  font-family: 'Raleway', sans-serif;
}
```

Show the changes and explain what you did.

---

### Navbar
Now add the following code inside the `HTML` box:

```html
<nav class="navbar">
  <ul>
    <li id="brand"><a href="#home" class="nav-link">Your Name</a></li>
    <li><a href="#contact" class="nav-link">Contact</a></li>
    <li><a href="#about" class="nav-link">About</a></li>
  </ul>
</nav>
```

Explain what `HTML` tags do, as well as the difference between `classes` and `ids`.  

Now, go to `CSS` and add the following, explaining as you build:

```css
nav {
  background-color: grey;
  position: fixed;
  top: 0;
  left: 0;
  height: 50px;
  width: 100vw;
  z-index: 1;
}

nav ul li {
  float: right;
  margin-right: 50px;
  list-style-type: none;
  text-align: center;
}

#brand {
  float: left;
}

.nav-link {
  color: darkred;
  text-decoration: none;
  font-family: 'Acme', sans-serif;
}

.nav-link:hover {
  color: lightblue;
  font-weight: bold;
}

#brand .nav-link {
  color: lightblue;
  font-size: 14pt;
}

#brand .nav-link:hover {
  color: darkred;
}
```

You should now have a fully-built navbar.

---

### Header
Now add the following to your `HTML`:

```html
<header id="home">
  <h1 class="header-tag">Nice to Meet You!</h1>
  <h3 class="header-tag">I'm the <i>CSS</i> to your <i>HTML</i></h3>
</header>
```

Explain things like header and i tags.

Add the following, then, to you `CSS`:

```css
h1 {
  font-size: 60pt;
  font-family: 'Acme', sans-serif;
}

#home {
  margin-top: 50px;
  position: relative;
  left: -8px;
  width: 100vw;
  height: 30vh;
  padding-top: 3em;
  /* Don't forget to have the class go choose an image for the background */
  background: url('https://images.unsplash.com/photo-1516821371801-280cf8069a4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1800&q=80') center 75% no-repeat fixed;
  background-size: cover;
}

.header-tag {
  text-align: center;
  color: darkred;
  text-shadow: 2px 2px 2px black;
}

h3.header-tag {
  margin-top: -30px;
  font-size: 18pt;
}
```

As you build, go to <a href="https://unsplash.com/">Unsplash</a> and explain why it is important to get pictures that are open source (no copyright).  

*NOTE:*  the `75%` in the `background` property is to push the image up 75% of the way, this allows you to see the mountains better for this example.  Start with `center center no-repeat fixed`, allowing the picture to be fully centered, not tiled, and not scrollable within the header tag.

---

### About
This section will require the most styling, fyi.

Add the following to your `HTML`:

```html
<div class="main">
  <section id="about">
    <div id="about-picture">
      <img src="./assets/img/profilePicture.jpg" alt="" id="profile-pic">
    </div>
    <div id="about-content">
      <h2>Your Name</h2>
      <!-- Have the class choose an ipsum off the internet, and explain what an ipsum is -->
      <p>Spicy jalapeno bacon ipsum dolor amet biltong bresaola tongue fatback brisket short loin. Brisket pancetta picanha boudin porchetta chicken, short ribs buffalo turducken kielbasa. Short ribs pork pork belly porchetta pastrami turducken. Shank fatback sausage flank corned beef pig buffalo porchetta short loin beef picanha meatloaf. Hamburger shank bresaola meatball sausage pastrami landjaeger tri-tip flank shoulder picanha bacon fatback pork belly. Capicola ham turkey t-bone, kevin shankle chicken buffalo picanha pig short loin bresaola. Landjaeger pig pastrami, pancetta swine biltong pork loin prosciutto kevin sausage t-bone.</p>
    </div>
  </section>
</div>
```

We are using <a href="https://baconipsum.com/">Bacon Ipsum</a>.  Go ahead and also have them add a profile picture from their computer or facebook or whatever and paste it into the `assets/img` folder.

Now, add the following to your `CSS`, explaining as you build:

```css
h2 {
  font-family: 'Acme', sans-serif;
  color: darkred;
}

.main {
  text-align: center;
}

#about {
  margin-top: 50px;
  display: inline-block;
}

#about-picture {
  width: 30vw;
  float: left;
}

#profile-pic {
  height: 300px;
  width: 300px;
  object-fit: cover;
  border-radius: 0.4em;
  box-shadow: 2px 2px 2px black;
}

#about-content {
  width: 40vw;
  float: right;
}
```

This will get you through the whole build, hopefully.

---

### Expanding
If for some reason you have time, feel free to add the contact section, using <a href="https://formspree.io/">Formspree</a> for the form.  You will likely not have time.

Good luck.
