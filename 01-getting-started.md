# Getting Started

## Lab 1a: _Hello, Vue!_

> Purpose: To get started with Vue.

1.  Create a new folder for your first project. Call it `hello-vue`.

2.  Inside it, create an `index.html` file. VS Code has a template, or you can use [this one](https://gist.github.com/petermunro/3ea1faf42553c9edb281b80d68d2627b).

3.  Import Vue by including this `<script>` element:

         <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>

    > This uses the development version of Vue. There's a separate production version which is optimised and minified.

4. In your HTML file, add a `<div>` with an `id` of `"app"`.
   Within the div, add an `<h1>` containing `{{ message }}`.
   This double-brace expression will be _interpolated_ by Vue:
   rewritten to display the value of the JavaScript `message` property.

5. Create a new `<script>` below the previous (`.../vue.js`) one.
   Add the following JavaScript:

        let app = new Vue({
            el: "#app",
            data: {
                message: "Hello, Vue!"
            }
        });

   Note how you're asking Vue to:

    1. supply the `data` your template will display, particularly the `message`; and
    2. treat the HTML element with the `id` of `"app"` (your `<div>`) as the place to render your template containing your data.

6. Check that the page renders correctly and that there are no errors in the console.


## Lab 1b: 

1. Have Vue render a page that resembles the following image:

    ![Visit the Christmas Lights Rendering](images/visit-the-christmas-lights-rendering.png)

    - The title (_"Visit the Christmas Lights"_), the location (_"Canary Wharf, London_") and the date (_"December"_) should be interpolated, but not the surrounding text.