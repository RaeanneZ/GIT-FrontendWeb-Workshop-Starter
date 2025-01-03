# GIT Frontend Workshop: Starter
## Overview
This document serves as a consolidated guide for the MUSE Café project, detailing the structure, content, constants, and color codes used in the HTML and CSS files. This will help developers and designers understand the project better and follow along easily.

## Project Structure
- HTML File: Contains the structure and content of the webpage.
- CSS File: Contains the styling and layout for the webpage.

## Content Overview
### Navbar Links
- Home
- Drinks
- About Us

### Carousel Products
1. **Cherry Blossom Latte**
    - **Title**: Spring in Every Sip
    - **Description**: Delight in the delicate flavors of spring with our Cherry Blossom Latte. A perfect blend of smooth espresso, creamy milk, and the floral sweetness of cherry blossoms. Topped with a dusting of pink sugar for a magical touch.
    -  **Cost**: Special: $12 for 2 | $8 for 1
    -  **Image**: `../images/cherryDrink.png`

2. **Mango Latte**
    - **Title**: Tropical Bliss
    - **Description**: Escape to paradise with every sip of our Mango Latte. A velvety mango puree blended with creamy milk and a hint of espresso, creating a tropical drink that’s both refreshing and indulgent.
    -  **Cost**: Special: $10 for 2 | $6 for 1
    -  **Image**: `../images/mangoDrink.png`

3. **Hot Cocoa**
    - **Title**: Comfort in a Cup
    - **Description**: Cozy up with our rich and creamy Hot Cocoa. Made with premium cocoa and steamed milk, this classic drink is topped with fluffy whipped cream and chocolate shavings for the ultimate treat.
    -  **Cost**:  Special: $8 for 2 | $5 for 1
    -  **Image**: `../images/chocoDrink.png`


### Shop Content
- **Title**: Welcome to MUSE Café
- **Description**: Step into a world of delightful aromas and comforting flavors. Our café is more than a place to grab a drink—it's a haven for relaxation, inspiration, and connection. Whether you're here for a quick latte or a leisurely chat, we're thrilled to have you.
- **Image**: `../images/shop.jpg`

### Footer
- **Copyright**: © 2024 MUSE Café. All Rights Reserved.
- **Social Links**:
    - Tiktok
    - Twitter
    - Instagram

## CSS Constants
### Font Families
- Primary Font: Poppins
- Fallback Font: sans-serif


### Color Codes
- Links Color: ![#555555](https://placehold.co/15x15/555555/555555.png)   `#555555`
- Hover Color: ![#FB9AAC](https://placehold.co/15x15/FB9AAC/FB9AAC.png)    `#FB9AAC`
- Divider Line Color: ![#333333](https://placehold.co/15x15/333333/333333.png)    `#333333`


### Carousel Product Transformations and Effects
```css

--prod1-transform: translate(-50%, -10%) scale(2)
--prod1-filter: blur(30px)
--prod1-zIndex: 11
--prod1-opacity: 0

--prod2-transform: translate(0, 0)
--prod2-filter: blur(0)
--prod2-zIndex: 10
--prod2-opacity: 1

--prod3-transform: translate(55%, 10%) scale(0.8)
--prod3-filter: blur(10px)
--prod3-zIndex: 9
--prod3-opacity: 1

--prod4-transform: translate(90%, 20%) scale(0.3)
--prod4-filter: blur(30px)
--prod4-zIndex: 8
--prod4-opacity: 0

```

### Footer Divider Line Gradient
```css

hr {
  width: 70%;
  height: 1.5px;
  justify-self: center;
  background: -webkit-gradient(
    linear,
    0 0,
    100% 0,
    from(rgba(0, 0, 0, 0)),
    color-stop(0.5, #333333),
    to(rgba(0, 0, 0, 0))
  );
  background: -webkit-linear-gradient(
    left,
    rgba(0, 0, 0, 0),
    #333333,
    rgba(0, 0, 0, 0)
  );
  background: -moz-linear-gradient(
    left,
    rgba(0, 0, 0, 0),
    #333333,
    rgba(0, 0, 0, 0)
  );
  background: -o-linear-gradient(
    left,
    rgba(0, 0, 0, 0),
    #333333,
    rgba(0, 0, 0, 0)
  );
  background: linear-gradient(
    left,
    rgba(0, 0, 0, 0),
    #333333,
    rgba(0, 0, 0, 0)
  );
  border: 0;
}

hr:after {
  /* For the gradient */
  display: block;
  content: "";
  height: 30px;
  background-image: -webkit-gradient(
    radial,
    50% 0%,
    0,
    50% 0%,
    116,
    color-stop(0%, #cccccc),
    color-stop(100%, rgba(255, 255, 255, 0))
  );
  background-image: -webkit-radial-gradient(
    center top,
    farthest-side,
    #cccccc 0%,
    rgba(255, 255, 255, 0) 100%
  );
  background-image: -moz-radial-gradient(
    center top,
    farthest-side,
    #cccccc 0%,
    rgba(255, 255, 255, 0) 100%
  );
  background-image: -o-radial-gradient(
    center top,
    farthest-side,
    #cccccc 0%,
    rgba(255, 255, 255, 0) 100%
  );
  background-image: radial-gradient(
    farthest-side at center top,
    #cccccc 0%,
    rgba(255, 255, 255, 0) 100%
  );
}

```
