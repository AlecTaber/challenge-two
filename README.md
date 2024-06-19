# My Portfolio

This is a webpage to my Portfolio that I will be continuing to add to after every project. It includes a section about me, links to my projects I have built and my contact information. The page is up to accessablity standards and has navigation links to all sections on the page. The webpage is meant to be easy to follow and has pictures with alt text related to my projects. The motivation behind this project was to learn about usuing CSS to build a readable portfolio for future employers seeking information about me and my work. I built this project to learn how to use flex boxes, media queries, and the CSS box model. I was given the CSS code for this project and needed to write HTML code to make the CSS function properly.

## Code Examples
This is the HTML code to get that navigation bar working on the webpage.
```html
<header>
        <h1>Alec Taber</h1>
        <nav>
            <a href="#page-section">About Me</a>
            <a href="#flex-item">Work</a>
            <a href="#contact-address">Contact Me</a>
            <a href="https://www.linkedin.com/in/alec-taber-11b963311/">Linkedin</a>
        </nav>
    </header>
```

This is the CSS code for the navigation bar.

```css
nav {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

nav a {
  text-decoration: none;
  padding: 5px 10px;
  color: var(--secondary);
  margin-right: 10px;
  background-image: linear-gradient(270deg, var(--secondary) 0%, var(--secondary) 100%);
  background-repeat: no-repeat;
  background-size: 100% 0.2em;
  background-position: bottom;
  transition: all 0.25s ease-in;
  font-size: 1.4rem;
}

nav a:hover {
  background-size: 100% 100%;
  color: var(--primary);
}

nav a:last-child {
  margin-right: 0;
}
```
This is the HTML code for the first item in the "Work" section of the page.

```html
<section class="flex-conatainer">
            <article class="flex-item">
                <div>
                    <h3>Accessability Standards</h3>
                    <a href="https://alectaber.github.io/challenge-one/">
                        <img src="images/HTML.jpg" alt="Large text that says HTML" height="100px">
                    </a>
                </div>
            </article>
```

The CSS code for this section needed to change the size of the first item compared to the rest of the items. This is the code for all the items in the "Work" section and the changes needed for the first item.

```css
.flex-item {
  border: 5px solid var(--secondary);
  background-color: var(--primary);
  color: var(--tertiary);
  min-height: 150px;
  max-height: 150px;
  flex-basis: calc(50% - 1em);
  display: flex;
  align-items: flex-end;
  padding: 0 0 20px 0;
  margin: 0.5em;
  text-decoration: none;
  background-blend-mode: soft-light;
  background-size: 150%;
  transition: all 0.5s;
  font-size: 0.9rem;
}

/* feature first portfolio item */
.flex-item:first-child {
    min-height: 400px;
    flex-basis: 100%;
}
```
This is the HTML code for the footer element conataining the contact information on the page.

```html
<footer class="contact-address">

    <a href="mailto:alectaber12@gmail.com">Email</a>
    <a href="https://github.com/AlecTaber">Github</a>

</footer>
```

This is CSS for the footer element.

```css
.contact-address {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  height: 100%;
}

.contact-address a {
  color: var(--tertiary);
  padding: 5px;
  text-decoration: none;
  font-size: 1.3rem;
  font-style: normal;
  background-image: linear-gradient(270deg, var(--primary) 0%, var(--primary) 100%);
  background-repeat: no-repeat;
  background-size: 100% 0.2em;
  background-position: bottom;
  transition: all 0.25s ease-in;
  margin: 0 0.2rem 0.1rem;
  display: inline-block;
}

.contact-address a:hover {
  background-size: 100% 88%;
  color: var(--secondary);
}
```
## Usage

## Built With

* [HTML](https://www.w3schools.com/html/default.asp)
* [CSS](https://www.w3schools.com/css/default.asp)

## Deployed Link

* [See Live Site](#)


## Authors

* **Alec Taber** 

- [Link to Portfolio Site](#)
- [Link to Github](https://github.com/AlecTaber)
- [Link to LinkedIn](https://www.linkedin.com/in/alec-taber-11b963311/)

## License

This project is licensed under the MIT License 

