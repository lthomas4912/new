# Responsive Design - Media Queries

**Approx. Time:** 45min

## Objective
Students will learn how to add breakpoints to the CSS using media queries

## Key Takeaways

* Correct Syntax
* General Breakpoints
* Max-width property
* `vw` unit of measure



## Media Query Steps

1. Open a project/workspace in Gitpod

2. Start the project using `npm start` or `yarn start`

3. Open the preview in another tab

4. Right-click and `Inspect` the web page

5. Next to the word `Element` is an icon to toggle the toolbar. Click it.

    * The browser can now be viewed responsively. The resolution can be adjusted via width and height. 

6. Change the width to `320px` and height. Observe the screen. Images and buttons are not responsive. Let's add a media query that makes the image responsive

7. Got to the CSS file for the app and go all the way to the bottom, to the last line of code. Add the media query there.

    ```html
    @media only screen and (max-width: 600px)
    ```
    
    * `max-width: 600px` is a breakpoint for screens that are 600px and less. 

    * One CSS rule that can be added is:

        ```html
        * {
        max-width: 100%;
        height: auto;
        }
        ```

    * This selects all elements and gives them a `max-width` set to 100%, meaning items will not scale up to be larger than the original size.

    * `height` set to `auto` makes all elements responsive and scale up and down

8. Next, let's resize an image. Select the class or Id of and image. Add the properties and values `max-width:100%;` and `height: auto;`.

    * The image is probably huge and takes up most of the screen. We need to adjust the percentage to make the image fit appropriately. Decrease the percentage to 30% and adjust. 

        * If the image has an inline CSS, the media query will not have any effect. Inline CSS rules take higher priority over rules in an external CSS.

9. Take note of the font-size. Is it bigger or smaller than before? Let's add a property and value using the `vw` unit of measure. Select a class or an Id that points to text.

    ```html

      .first-title {
        font-size: 1vw;
      }
    ```

    * Setting the `font-size` to `1vw` makes the size 1% of the viewport. Increase the measurement to see what works best. 

10. Continue to add CSS rules to the media query to ensure the elements are scaled appropriately.

11. Let's add another breakpoint for tablets and large phones with a width of `600px` and up.

    ```html
    @media only screen and (min-width: 600px)
    ```

12. Add CSS rule to ensure the elements on the screen are scaled and positioned correctly.


### Additional Goals 

* Continue to add breakpoints with media queries and CSS rules for various viewport widths. 

    * Devices `768px` and up (landscape tablets)

    * Devices `992ox` and up (laptops/desktops)

    * Devices `1200px` and up (large laptops and desktops)