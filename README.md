
💻 HTML & CSS Project Log
Week Overview: Deep Dive into CSS, Flexbox & Sass
I'm currently working on a front-end development project focused on improving my skills in CSS, Flexbox, and Sass. This course has been incredibly helpful, as it's not just theory—we're actually building a full website. It’s a hands-on way to practice advanced CSS concepts and work with Sass in more detail.

🧠 Learning Sass
Sass (Syntactically Awesome Stylesheets) is a powerful CSS preprocessor. It's like an extension of CSS that brings added functionality and cleaner syntax to your stylesheets.

Here are the key Sass features I've been working with:

Variables – Store reusable values like colors, font sizes, and spacing.

Nesting – Allows selectors to be nested inside each other, resulting in more readable code.

Operations – Perform mathematical operations directly in your stylesheets.

Partials & Imports – Break code into smaller files and import them into a main stylesheet.

Mixins – Reusable chunks of code that can be included wherever needed.

Functions – Similar to mixins, but return values.

Extend – Share a set of CSS properties from one selector to another.

⚙️ Project Setup: Node.js & NPM
To compile Sass and manage dependencies, I’ve been using Node.js and NPM. Here’s a quick breakdown of what I did:

Initialize the project:

bash
Copy
Edit
npm init
This created a package.json file to manage project dependencies.

Install Sass compiler:

bash
Copy
Edit
npm install node-sass --save-dev
Create a Sass compile script:
In package.json, I added a script:

json
Copy
Edit
"scripts": {
  "compile:sass": "node-sass sass/main.scss css/style.css -w"
}
The -w flag tells Sass to watch for changes and recompile automatically.

✅ After some debugging (including fixing a folder name issue that took hours 😅), I finally got the compile command running!

🗂️ Sass File Structure
To keep my project organized and scalable, I split Sass code into multiple folders and files. Here's how I structured the imports in the main main.scss:

scss
Copy
Edit
@import "abstracts/functions";
@import "abstracts/mixins";
@import "abstracts/variables";

@import "base/base";
@import "base/animations";
@import "base/typography";
@import "base/utilities";

@import "pages/home";
Each folder handles specific responsibilities—this makes the code much easier to maintain and understand.

🖼️ Example Sass Code
scss
Copy
Edit
.header {
  height: 95vh;
  background-image: linear-gradient(
      to right bottom,
      rgba(209, 10, 10, 0.15),
      rgba(144, 144, 195, 0.65)
    ),
    url(/image/rsz_viator_shutterstock_186247-1200x809.webp);
  background-size: cover;
  background-position: top;
  position: relative;
  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);

  &__logo-box {
    position: absolute;
    top: 4rem;
    left: 4rem;
  }

  &__logo {
    height: 4.5rem;
  }

  &__text-box {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
}
Note how the &__ syntax makes it easy to keep class names modular and readable.

🔧 Tools & Resources
🎨 Adobe Color Wheel – For creating beautiful color palettes.

🌈 Color Safe – Ensures text contrast and accessibility.

🧪 Code Editor: VS Code

🔧 Terminal for running NPM scripts

🧠 Mindset & Motivation
I've made a commitment to practice coding every day, even if it's just for 20–30 minutes. Some days are harder than others—yes, I’ve felt down—but I keep reminding myself: progress over perfection.
Today I chose me. I'm investing in my future, learning something valuable, and pushing through the tough parts. 💪

🏁 Goals
Finish the Sass project by the end of this week.

Log at least 8 hours of focused learning.

Stay consistent—30 minutes minimum of daily practice.

🚀 Final Thoughts
This project has been a rollercoaster—frustrating bugs, breakthrough moments, and real progress. I’m learning, building, and growing. Can't wait to see where this journey takes me next.

Let’s keep going! 👨‍💻🔥

still here

